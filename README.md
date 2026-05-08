# Assignment 2

## 24324533 - CITS4407 Assignment 2


This repository contains the code for Assignment 2 of the CITS4407 Open Source Tools and Scripting course.

## Script 1: clean

This script validates and cleans the raw trending YouTube videos dataset.

Features:
- Checks for missing input files
- Validates CSV format
- Detects empty files
- Verifies correct column count
- Removes duplicate rows
- Removes rows with missing required values
- Removes rows with zero likes or dislikes
- Removes the ratings_disabled column
- Cleans publish_date values by removing timestamps

Setup:
chmod +x clean

Usage:
./clean trending_videos_unclean.csv

Output:
Creates trending_videos_clean.csv

## Script 2: analyse

This script analyses the cleaned trending videos dataset.

Features:
- Finds the most frequent video ID
- Calculates the mean number of views
- Finds the video with the maximum dislikes
- Calculates the highest engagement rate
- Calculates the least net sentiment rate
- Handles ties clearly in the output

Setup:
chmod +x analyse

Usage:
./analyse trending_videos_clean.csv

Output:
Prints the analysis results to standard output.

Example output:
Most frequent video, ID: id4667
Mean number of views: 2355595.97
Max dislikes video, ID: id2798
Highest engagement rate video, ID: id2282, dated: 2018-01-04
Least sentiment rate video, ID: id2219, dated: 2017-12-13

## Files

- clean
- analyse
- trending_videos_unclean.csv
- trending_videos_clean.csv

## Notes

- Developed using Bash and Unix tools covered in the unit.
- Tested using the provided Docker image.
- Git is used throughout development with multiple commits.