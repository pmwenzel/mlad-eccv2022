# MLAD ECCV 2022 Localization Challenge

For the localization challenge, we provide three different scenarios, each consisting of a reference map and a query sequence from the [4Seasons](https://www.4seasons-dataset.com/) dataset. 

1. City Loop
  * reference map: `city_loop_2_train`
  * query sequence: `city_loop_2_test`
2. Old Town
  * reference map: `old_town_2_train`
  * query sequence: `old_town_3_test`
3. Parking Garage
  * reference map: `parking_garage_2_train`
  * query sequence: `parking_garage_1_test`

Each reference map contains highly accurate reference poses. All sequences from the [4Seasons](https://www.4seasons-dataset.com/) dataset can be used as training data.

## Dataset Download

To download the challenge data and other sequences from the dataset, we refer to the [download](https://www.4seasons-dataset.com/dataset) page.

## Dataset Structure

For details on the dataset structure, we refer to the following [documentation](https://www.4seasons-dataset.com/documentation).

## Libartipy Python Library

In this [repository](https://github.com/Artisense-ai/libartipy), you will find a set of tools for working with the 4Seasons dataset.

## Task

Each `reloc_source_to_target.txt` contains a list of first the keyframe from the source (reference) sequence and the query keyframe. The task is to provide the relative pose between the source and the query frame. Note that the relative pose is from cam0 of the reference sequence to cam0 of the query sequence, respectively. The `6DOF` poses are specified as translation (`t_x`, `t_y`, `t_z`), and quaternion (`q_x`, `q_y`, `q_z`, `q_w`).

## Submission

For the test sequences, the ground truth is withheld. For submitting your results to the challenge, please refer to the steps described at: [https://sites.google.com/view/mlad-eccv2022/challenge](https://sites.google.com/view/mlad-eccv2022/challenge).