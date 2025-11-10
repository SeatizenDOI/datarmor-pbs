# ODM

Be mindful of the **ODM version** you use.
All my orthophotos were generated with [**ODM 3.5.3**](https://github.com/OpenDroneMap/ODM/releases/tag/v3.5.3).

I observed that processing parameters differ between **drone** and **ASV** datasets, so I created separate folders to keep them organized.

I didn’t perform 3D reconstruction — instead, I used the **`fast-ortho`** parameters, which produce orthophotos more efficiently and with better results for my use case.

You’ll need to **build a Singularity container** from the provided Docker image.

I don’t use **GPU acceleration**, since the GPU is only used for SIFT feature extraction.
The **GPU queue walltime** on Datarmor is limited to **72 hours**, while some reconstructions can take over **100 hours**.
By using the **OMP queue**, I can allocate **more RAM and CPU cores**, which improves performance for large datasets.

