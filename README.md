# Tuple Space Travel Route

## Basic Premise

A spacecraft has been assigned a fixed travel route. Once the mission begins, the destinations should not be changed, making a tuple a good way to store the route.

Your program will use a provided tuple and display information about the mission.

The program will begin with:

```python
mission_route = (
    "Earth",
    "Luna Station",
    "Mars",
    "Europa",
    "Titan",
    "Neptune Station"
)
```

## Basic File Structure

```text
basic/
└── main.py
```

## Basic Requirements

* [ ] Use the provided `mission_route` tuple without adding, removing, or changing any of its values.
* [ ] Display the **first destination** and **last destination** by accessing their indices.
* [ ] Use `len()` to display the total number of destinations in the route.
* [ ] Use a `for` loop to display every destination in the order it will be visited.
* [ ] Use `in` to check whether `"Europa"` is included in the route and display an appropriate message.

> Fully completing the Basic Requirements earns **16/20 marks, or 80%**.

## Basic Assessment — 16 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| Tuple Usage | Uses the provided tuple without attempting to modify its contents. | 3 |
| Index Access | Correctly accesses and displays the first and last destinations. | 3 |
| Tuple Length | Correctly uses `len()` to determine and display the number of destinations. | 3 |
| Traversing the Tuple | Uses a `for` loop to display every destination in order. | 4 |
| Membership Check | Uses `in` to determine whether Europa is part of the route and displays the result. | 3 |
|  | **Total** | **16** |

## Advanced Premise

Extend the Basic program so that the user can enter the name of a destination and receive information about where that destination appears in the fixed mission route.

The `mission_route` tuple should remain unchanged. The program should use the information already stored in the tuple to determine the destination's position within the journey.

Students can begin by copying their completed Basic program into the Advanced folder.

## Advanced File Structure

```text
advanced/
└── main.py
```

## Advanced Requirements

* [ ] Use `input()` to ask the user for the name of a destination and confirm whether or not that destination exists in `mission_route`.
* [ ] If the destination exists, determine and display how many **stops away from the start** of the journey it is. The first destination is `0` stops away from the start.
* [ ] Determine and display how many **stops away from the end** of the journey the destination is. The final destination is `0` stops away from the end.
* [ ] If the selected destination is not the final destination, display the **next stop** in the journey.
* [ ] If the destination does not exist, display an appropriate message instead of attempting to calculate its position or next stop.

For example, using the provided route:

```python
mission_route = (
    "Earth",
    "Luna Station",
    "Mars",
    "Europa",
    "Titan",
    "Neptune Station"
)
```

A user searching for:

```text
Mars
```

could receive:

```text
Mars is part of the mission route.
Stops from start: 2
Stops from end: 3
Next stop: Europa
```

A user searching for:

```text
Neptune Station
```

could receive:

```text
Neptune Station is part of the mission route.
Stops from start: 5
Stops from end: 0
This is the final stop of the journey.
```

## Advanced Assessment — 4 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| Destination Search | Accepts a destination from the user and correctly determines whether it exists in the mission route. | 1 |
| Position from Start | Correctly determines and displays how many stops the destination is from the beginning of the journey. | 1 |
| Position from End | Correctly determines and displays how many stops the destination is from the end of the journey. | 1 |
| Next Stop | Correctly displays the next destination when one exists and appropriately handles the final destination. | 1 |
|  | **Total** | **4** |