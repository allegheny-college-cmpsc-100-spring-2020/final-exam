# CMPSC 100-02: Final Code Option (100 pts.)

**NOTE: You are only required to complete one of the Final options; if choosing to do both, you will receive the higher>
* Assigned: 27 April, 2020
* Due: 5 May 2020 at **12:00 AM** (this would have been the end of our normally-scheduled exam time)
* Point value: 100 pts

## Activity: Widget Factory reprise

The `code` directory contains a class (`Widget.java`) and a driver file (`MakeWidgets.java`).

| Task                                                                       | Point Value                |
|----------------------------------------------------------------------------|----------------------------|
| Implement a `constructor`                                                  | 10 pts.                    |
| Implement "getter" methods to return Widget `name`,`price`, and `weight`   | 30 pts.                    |
| Collect objects in a data structure                                        | 10 pts.                    |
| Correct output                                                             | 50 pts.                    |
| Total prices and weights                                                   | 10 pts. (extra credit)     |

`gradle grade` and `gradle build` are available.

## Implement a constructor: `Widget.java` (10 points)

A `Widget`, for the purposes of this problem, is an object with three features:

* name
* weight
* price

To properly create a `Widget`, these features need to be provided at object creation using a `constructor` method such that:

```java
Widget widget = new Widget("Thingamajig",13.37,42.12);
```

represents a correct and complete instantiation/creation of a `Widget` object.

These attributes should be accessible outside of the `Widget` class, but be unalterable beyond their assignment in the `constructor`.

## Implement "getter" methods to return `Widget` `name`, `price`, and `weight`: `Widget.java` (30 pts.)

For each instance variable in the `Widget` object, write a "getter" to return the value of given object's `name`, `price`, and `weight` such that your `MakeWidgets` code can call them.

## Collect objects in a data structure: `MakeWidgets.java`  (10 points)

`Widget` objects should be packed into a data structure called `crate`, which contains 5 `Widget` objects. Iterating over this crate object should enable creation of successful output.

## Correct output (50 points)

In the `MakeWidgets.java` file, when iterating over the `crate` data stucture, the program should print each `Widget` such that a list appears in the following format:

```
There are 5 widgets in this crate:

$13.37  42.12 kilograms Thingamajig
$19.79  34.23 kilograms Zonk
$18.94  12.21 kilograms Maguffin
$13.37  97.97 kilograms Whatchamacallit
$119.34 41.12 kilograms Gadget
```

## Extra Credit (10 points)

In an effort to make our `Widget` factory more efficient, we might choose to add labels to the crates. Beneath the print-out from the previous step, implement an additional line so that the output looks like the following:

```
There are 5 widgets in this crate:

$13.37  42.12 kilograms Thingamajig
$19.79  34.23 kilograms Zonk
$18.94  12.21 kilograms Maguffin
$13.37  97.97 kilograms Whatchamacallit
$119.34 41.12 kilograms Gadget

------- ------
$184.81 227.65 kilograms
```
