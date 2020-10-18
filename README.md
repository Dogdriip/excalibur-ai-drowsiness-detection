# Drowsiness Detection

## Build

```sh
$ pyinstaller blink_video.py --onefile --hidden-import sklearn.neighbors.typedefs --hidden-import sklearn.neighbors.quad_tree --hidden-import sklearn.tree._utils
```

## Exec

Be sure `shape_predictor_68_face_landmarks.dat`, 'Trained_SVM_C=1000_gamma=0.1_for 7kNegSample.sav' are in ./dist/

```sh
$ ./dist/blink_video <VIDEO_PATH>
```

