# Tensorflow Version Update to v2.3.0

### Due to pip upgrade of next-generation dependency resolver there are issues getting observed on installing Tensorflow latest version. Following code will solve this error, and let you update Tensorflow.

 1. ERROR: No matching distribution found for tensorboard<2.2.0,>=2.1.0 (from tensorflow).
 2. ERROR: tensorflow-gpu 1.14.0 requires tensorboard<1.15.0,>=1.14.0, but you'll have tens
 orboard 2.3.0 which is incompatible.
 3. Suggestion to use : --use-feature=2020-resolver
 
 ### Use following code block to solve the issue,
 `!pip install --user tb-nightly`
 
`!python -m pip install --upgrade pip`

`!pip check`

`!pip install --user tensorflow --use-feature=2020-resolver`
