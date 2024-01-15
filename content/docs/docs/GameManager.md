+++
title = "GameManager"
description = "Klasa odpowiadająca za zarządzanie serwerem, grą i graczami."
author = "wzimongus"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node](../Node)

## Description

Klasa odpowiadająca za zarządzanie serwerem, grą i graczami.

## Constants Descriptions

### ERROR\_MESSAGES

```gdscript
const ERROR_MESSAGES: Dictionary = {"ERR_CLIENT":"Nie udało się utworzyć klienta! Powód: %s","ERR_CONNECTION":"Nie udało się połączyć z %s!","ERR_CONNECTION_FAILED":"Nie można połączyć się z serwerem!","ERR_CONNECTION_LOST":"Połączenie z serwerem zostało przerwane!","ERR_GAME_STARTED":"Gra już się rozpoczęła!","ERR_LOBBY_NAME_LENGTH":"Nazwa lobby musi mieć od 3 do 16 znaków!","ERR_MAX_PLAYERS":"Przekroczono limit graczy!","ERR_PORT":"Nie udało się nasłuchiwać na porcie %s!","ERR_SERVER":"Nie udało się uruchomić serwera!","ERR_USERNAME_LENGTH":"Nazwa użytkownika musi mieć od 3 do 16 znaków!"}
```

Komunikaty błędów.

### Role

```gdscript
enum Role{STUDENT = 0, LECTURER = 1}
```

Rola gracza.

### SKINS

```gdscript
const SKINS: Dictionary = {"0":{"name":"Alternatywka","resource":"res://assets/textures/skins/alternatywka_spritesheet.png"},"1":{"name":"Barbie","resource":"res://assets/textures/skins/barbie_spritesheet.png"},"2":{"name":"Ecoświr","resource":"res://assets/textures/skins/ecoswir_spritesheet.png"},"3":{"name":"Femboy","resource":"res://assets/textures/skins/femboy_spritesheet.png"},"4":{"name":"Gamer","resource":"res://assets/textures/skins/gamer_spritesheet.png"},"5":{"name":"Gymbro","resource":"res://assets/textures/skins/gymbro_spritesheet.png"},"6":{"name":"Hipster","resource":"res://assets/textures/skins/hipster_spritesheet.png"},"7":{"name":"Nerd","resource":"res://assets/textures/skins/nerd_spritesheet.png"},"8":{"name":"Punk","resource":"res://assets/textures/skins/punk_spritesheet.png"},"9":{"name":"Rasta","resource":"res://assets/textures/skins/rasta_spritesheet.png"},"10":{"name":"TikToker","resource":"res://assets/textures/skins/tiktoker_spritesheet.png"},"11":{"name":"Wixiarz","resource":"res://assets/textures/skins/wixiarz_spritesheet.png"}}
```

Dostępne skiny.

## Property Descriptions

### is\_game\_scene\_loaded

```gdscript
var is_game_scene_loaded: bool = false
```

Przechowuje informacje o stanie gotowości sceny gry.

### lobby\_data\_at\_registration

```gdscript
var lobby_data_at_registration
```

Przechowuje dane innych graczy z momentu rejestracji, w celu zespawnowania ich w lobby.

### is\_meeting\_called

```gdscript
var is_meeting_called: bool = false
```

Okrśla czy jest zwołane alarmowe zebranie.

### is\_animation\_playing

```gdscript
var is_animation_playing: bool = false
```

Przechowuje informacje o tym czy animacja tła jest w trakcie odtwarzania.

### animation\_position

```gdscript
var animation_position: float
```

Przechowuje pozycję animacji tła.

### wait\_time

```gdscript
var wait_time
```

Przechowuje czas oczekiwania na animację - potrzebny do przejść między scenami.

### current\_background\_texture

```gdscript
var current_background_texture = null
```

Przechowuje teksturę obecnego tła.

### transition\_background\_texture

```gdscript
var transition_background_texture = null
```

Przechowuje teksturę tła przejścia.

### is\_first\_time

```gdscript
var is_first_time: bool = true
```

Czy scena jest włączana po raz pierwszy.

### is\_sabotage

```gdscript
var is_sabotage: bool = false
```

Określa czy właśnie odbywa się sabotaż.

## Method Descriptions

### create\_lobby

```gdscript
func create_lobby(lobby_name: String, port: int)
```

Tworzy nowy serwer gry.

### change\_server\_settings

```gdscript
func change_server_settings(max_players: int, max_lecturers: int, kill_cooldown: int, sabotage_cooldown: int, kill_radius: int, task_amount: int, emergency_cooldown: int, student_light_radius: int, lecturer_light_radius: int, voting_time: int, discussion_time: int)
```

Zmienia ustawienia serwera.

### join\_lobby

```gdscript
func join_lobby(address: String, port: int)
```

Dołącza do istniejącego serwera gry.

### start\_game

```gdscript
func start_game()
```

Rozpoczyna grę.

### end\_game

```gdscript
func end_game()
```

Kończy grę.

### reset\_game

```gdscript
func reset_game()
```

Resetuje grę.

### new\_round

```gdscript
func new_round()
```

Rozpoczyna nową rundę.

### get\_current\_game\_value

```gdscript
func get_current_game_value(key: String)
```

Zwraca informację o grze, która jest przechowywana pod danym kluczem.

### set\_current\_game\_value

```gdscript
func set_current_game_value(key: String, value)
```

Zmienia informację o grze, która jest przechowywana pod danym kluczem.

### add\_vote

```gdscript
func add_vote(id: int, voted_by: int)
```

Dodaje głos do tablicy głosów.

### set\_most\_voted\_player

```gdscript
func set_most_voted_player(player)
```

Ustawia gracza z największą ilością głosów.

### get\_registered\_players

```gdscript
func get_registered_players()
```

Zwraca słownik zarejestrowanych graczy.

### get\_registered\_player\_value

```gdscript
func get_registered_player_value(id: int, key: String)
```

Zwraca informację o danym graczu, która jest przechowywana pod danym kluczem.

### get\_current\_player\_id

```gdscript
func get_current_player_id()
```

Zwraca ID obecnego gracza.

### get\_current\_player\_value

```gdscript
func get_current_player_value(key: String)
```

Zwraca informację o obecnym graczu, która jest przechowywana pod danym kluczem.

### set\_current\_player\_value

```gdscript
func set_current_player_value(key: String, value)
```

Zmienia informację o obecnym graczu, która jest przechowywana pod danym kluczem.

### get\_server\_settings

```gdscript
func get_server_settings()
```

Zwraca informacje o ustawieniach serwera.

### set\_pause\_menu\_status

```gdscript
func set_pause_menu_status(is_paused: bool)
```

Zmienia status informacji o wyświetlaniu menu pauzy.

### set\_input\_disabled\_status

```gdscript
func set_input_disabled_status(is_input_disabled: bool)
```

Zmienia status sterowania obecnego gracza.

### emit\_input\_status

```gdscript
func emit_input_status()
```

Emituje sygnał informujący o statusie sterowania.

### change\_skin

```gdscript
func change_skin(skin: int)
```

Zmienia skin obecnego gracza.

### async\_condition

```gdscript
func async_condition(cond: Callable, timeout: float = 10) -> Error
```

Asynchronicznie czeka na warunek.

### kill\_victim

```gdscript
func kill_victim(victim_id: int)
```

Zabija ofiarę.

### kill\_player

```gdscript
func kill_player(player_id)
```

Zabija gracza.

### check\_winning\_conditions

```gdscript
func check_winning_conditions()
```

Sprawdza warunki wygranej i emituje sygnał wygranej, jeśli któryś z warunków wygranej jest spełniony.

### teleport\_players

```gdscript
func teleport_players()
```

Teleportuje wszystkich graczy do miejsca spotkania.

### main\_map\_load\_finished

```gdscript
func main_map_load_finished()
```

Emituje sygnał po zakończeniu wczytywania.

### request\_light\_sabotage

```gdscript
func request_light_sabotage()
```

Przyjmuje prośbę o włączenie sabotażu.

### activate\_light\_sabotage

```gdscript
func activate_light_sabotage()
```

Emituje sygnał włączenia sabotażu.

### emit\_sabotage\_started

```gdscript
func emit_sabotage_started(has_started: bool)
```

Emituje sygnał informujący o rozpoczęciu/zakończeniu sabotażu.

### execute\_action

```gdscript
func execute_action(action_name: String)
```

Symuluje wciśnięcie klawisza w celu wywołania konkretnej akcji.

## Signals

- signal player_registered(id, player): Emitowany po zarejestrowaniu nowego gracza.
- signal player_deregistered(id, player): Emitowany po wyrejestrowaniu gracza.
- signal skin_changed(id, skin): Emitowany po zmianie skina gracza.
- signal input_status_changed(is_paused): Emitowany po zmianie statusu sterowania.
- signal registered_successfully(): Emitowany u klienta po jego pomyślnej rejestracji.
- signal game_started(): Emitowany po rozpoczęciu gry.
- signal game_ended(): Emitowany po zakończeniu gry.
- signal next_round_started(): Emitowany po zaczęciu nowej rundy.
- signal error_occured(message): Emitowany po wystąpieniu błędu.
- signal player_killed(player_id, is_victim): Emitowany po zabiciu gracza.
- signal sabotage_occured(): Emitowany po włączeniu sabotażu.
- signal sabotage_started(has_started): Emitowany po rozpoczęciu/zakończeniu sabotażu.
- signal map_load_finished(): Emitowany po zakończeniu ładowania mapy głównej.
- signal server_settings_changed(): Emitowany po zmianie ustawień serwera.
- signal winner_determined(winning_role): Emitowany gdy przynajmniej jeden z warunków zakończenia gry jest spełniony.
