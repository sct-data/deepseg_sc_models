sct_deepseg_sc models
===============================================================================

This folder contains the sct_deepseg_sc models:
- dwi_seg_sc.h5 trained on a private dataset including 94 subjects
- t1_seg_sc.h5 trained on a private dataset including 116 subjects
- t2s_seg_sc.h5 trained on a private dataset including 755 subjects
- t2_seg_sc.h5 trained on a private dataset including 840 subjects

This dataset includes healthy controls and patients with multiple sclerosis, amyotrophic lateral sclerosis, degenerative cervical myelopathy, traumatic spinal cord injury, neuromyelitis optica, and syringomyelia.

This dataset was created on 10 Dec 2017.

Images used for the models' trainings are listed in dataset.pkl:
      center contrast contrast_foldname patho                      subject  train_valid_test
0        amu       t1                t1   DCM   amu_2017-virginie_20140317               1.0
1        amu       t1                t1   SYR   amu_2017-virginie_20140505               1.0
2        amu       t2                t2   DCM   amu_2017-virginie_20170118               1.0
3        amu       t2                t2    MS         amu_2017-virginie_AS               1.0
4        amu      t2s           t2s_inf    MS         amu_2017-virginie_AS               1.0

... where the columns are:
- center: acquisition center
- contrast: image contrast used in sct_deepseg_sc
- contrast_foldname: folder name in the private dataset
- patho: abbrevation of the clinical status of each scanned subject, e.g., HC for Healthy control, MS for Multiple sclerosis
- subject: subject's ID
- train_valid_test: integer indicating in which sub-dataset this image has been used: 1 for training, 2 for validation, 3 for testing


Changelog
===============================================================================

2018-06-10 (included in v3.2.1):
- Added 3D models.

2018-02-12:
- Added readme with dataset descriptions.

2017-12-18:
- Models creation.
