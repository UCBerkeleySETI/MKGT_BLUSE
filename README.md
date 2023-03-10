# MeerKAT Grand Tour - BLUSE (SETI) Notebooks

This is the table of contents for the BLUSE notebooks used for the MeerKAT
Grand Tour workshop held at Rhodes University in Makhanda, Eastern Cape, South
Africa in January 2023.

1. Voyager tutorials

   The *Voyager 1* and *Voyager 2* space probes emit extraterretrial
   technosignatures near 8.4 GHz.  Despite being human-created, these signals
   are very useful as SETI test signals.  If we can't detect these
   human-created technosignatures, we are unlikely to be able to detect
   ET-created technosignatures.  Fortunately, we can detect Voyager and you can
   too using these notebooks!

   1. [`voyager_notebook_1.ipynb`](voyager/voyager_notebook_1.ipynb) Voyager 1 data from the GBT
   2. [`voyager_notebook_2.ipynb`](voyager/voyager_notebook_2.ipynb) Voyager 2 data from the Murriyang telescope (Parkes)
   3. [`voyager_notebook_3.ipynb`](voyager/voyager_notebook_3.ipynb) Voyager 1 data from the GBT, with *turboSETI*


2. `setigen` notebook

   [`setigen`](https://setigen.readthedocs.io/en/main/getting_started.html) is
   used to generate spectrogram data with embedded Doppler drifting signals as
   well as injecting simulated Doppler drifting signals into "real" data.  This
   gives is a way to test our Doppler drifting detection algorithms (e.g.
   *turboSETI*).  `setigen` can also inject RFI-like signals to give the
   simulated data a more realistic feel.

   You will use this `setigen` notebook to make your own simulated data with
   (or without if you prefer) Doppler drifting signals.  This notebook will get
   you started with `setigen`, but you are encouraged to experiment and get
   creative with the signals you choose to inject!

   [`setigen_notebook_1.ipynb`](setigen/setigen_notebook_1.ipynb)

   This notebook can save your simulated data (with injected signals) to disk
   so that you can exchange data files with your peers for use with the
   `turboSETI` notebook.


3. `turboSETI` notebook

   [`turboSETI`](https://turbo-seti.readthedocs.io/en/latest/) is a tool for
   detecting Doppler drifting signals in radio spectrogtrams (e.g. Filterbank
   files).  If one has several ON/OFF observations, `find_event_pipeline` can
   be used to determine whether "hits" are interesting (i.e. not consistent
   with RFI) or non-interesting (i.e. consistent with RFI).

   You will use this `turboSETI` notebook to search for Doppler drifting
   signals in data files that another student created using the `setigen`
   notebooks.  The data files that you created with the `setigen` notebooks
   will be searched by another student using these same notebooks.

   [`turboseti_1.ipynb`](turboseti/turboseti_1.ipynb)

   Can you and your peers detect each other's simulated signals?  Can you
   detect your own?
