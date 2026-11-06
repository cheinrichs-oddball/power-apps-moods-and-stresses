# Moods and Stresses (Power Apps)


As a health care provider, we are concerned with the moods and stress levels of our patients. We want to examine our data to determine who is likely not doing well based on our readings.

## Data Dictionary

### Users

The [users.csv](users.csv) file contains a list of users with `user_name` and `full_name` fields.

`user_id`, `user_name`, `full_name`

### Moods

In the [moods.csv](moods.csv) file, we have a daily log of each user's mood. The `mood` column evaluates them between 1 (very bad) and 5 (great). If a user's value is missing on a given day, we should default to a 3 (neutral).

`user_id`, `date`, `mood`

### Stress

the [stress.csv](stress.csv) file similarly contains a daily log of the person's stress level. A value of 1 indicates low stress, while a value of 5 indicates very stressed.

`user_id`, `date`, `stress`

## Requirements

### Part 1:

Use AI to read in the three data files using the language or framework of your choice.

### Part 2:

Without using AI, write a script or program to show:

- All users who had two or more bad days in the week beginning 2017-05-07, displaying their username and the number of bad days that week. The list should be ordered descending by number of bad days.
- The 5 longest streaks of consecutive bad days across the entire dataset. It should display the username and their consecutive bad day streak, ordered descending by length of streak.

A "bad day" is defined as a user's mood being in the 1-2 range or where their mood is a 3 and stress level is in the 4-5 range.

### Part 3:

Using AI, build some sort of front-end component to visualize the results of both prompts from Part 2.
