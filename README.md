**.fptab File Format**

The `.fptab` file format is a simple, text-based format for representing guitar tablature. Each line represents a string on the guitar, with the following format:

`FRET_NUMBER|FRET_FINGER|PICK_FINGER`

Where:

* `FRET_NUMBER`: The fret number to press down on the string (0 means play open string).
* `FRET_FINGER`: The left-hand finger to use for pressing the fret (1 = index, 2 = middle, 3 = ring, 4 = pinkie).
* `PICK_FINGER`: The right-hand finger to use for picking (0 = thumb, 1 = index finger).

**How to Read the File**

To read the file, follow these steps:

1. **Identify the strings**: Each line represents a string on the guitar, from top to bottom: E, B, G, D, A, E (low to high).
2. **Break down each note**: For each note, read the `FRET_NUMBER`, `FRET_FINGER`, and `PICK_FINGER` values from left to right.
3. **Play the notes**: Use the specified fingers to press the frets and pick the strings.

**Special Notes**

* **"X"**: If you see an "X" in the file, it means to play the string open, without pressing any fret.
* **Multiple notes at once**: If you see multiple notes on the same string, play them simultaneously using the specified fingers.

**Example**

Here's an example `.fptab` file:
```
e|---5|4|3|---3|2|2|
B|--------|--------|
G|--------|--------|
D|--------|---2|1|0|
A|---0|X|0|--------|
E|--------|--------|
```

**Example Breakdown**

Let's break down the first two notes:

1. **First note (2 notes at the same time)**:
	* Play the open A string with your thumb (right-hand finger 0).
	* Play the 5th fret on the high E string with your pinkie (left-hand finger 4) and pick with your ring finger (right-hand finger 3).
2. **Second note (2 notes at the same time)**:
	* Play the 2nd fret on the D string with your index finger (left-hand finger 1) and pick with your thumb (right-hand finger 0).
	* Play the 3rd fret on the high E string with your middle finger (left-hand finger 2) and pick with your 2nd finger (right-hand finger 2).