# Eluvio ML Challenges

## Scene Segmentation

Requirements:

* Python 3.9.1
* NumPy v1.20.0
* scikit-learn 0.24.1

Evaluate your predictions:

* In each `<imdb id>.pkl` we provided, `"scene_transition_boundary_ground_truth"` and `"scene_transition_boundary_prediction"` give the ground-truths and predictions from a pre-trained model. Each entry of a ground-truth or prediction array represents a shot transition, whose value indicates if it is a scene transition, or the probability of scene transition.  
* To evaluate the provided predictions, place `<imdb id>.pkl` for all movies in the dataset under `data_dir`, and run `evaluate_mscenes.py`:

```
python evaluate_mscenes.py $data_dir
```

* Note the fields needed for evaluation are `"scene_transition_boundary_ground_truth", "scene_transition_boundary_prediction", "shot_end_frame", "imdb_id"`. To evaluate your own predictions, store these data in the same format as above then run `evaluate_mscenes.py`.
