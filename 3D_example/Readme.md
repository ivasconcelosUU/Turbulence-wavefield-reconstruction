# Document desctrpition:

3D_recon.py: 3D reconstruction script, including cross derivatives and masks. 
	Notice: the dataset range will somehow affect the reconstruction result, default range was tested to have good reconstruction.
			The dataset is read from rsf files, change it if you want to use your own dataset. Or if you want to use the existing dataset, you probally need to change the header files (the description on directory), to make the rsf readable. 
			These messgages applied to any of the 3D reconstrction example.

3D_recon_nomask.py: 3D reconstruction without masks (in x-t and f-k domain), for the purpose of comparison.

3D_recon_nocross.py: 3D reconstruction without cross-derivatives, for the purpose of comparison.

idr_14.npy: an example of irregular sampling(1/4 decimation), an array of the sampled receiver numbers, to compare different reconstruction from the same sampling shceme.

3d_plotting.ipynb: an ipython notebook to plot the result, nothing important.

slurm-3.sh: a simple example of slurm script to run *.py on eejit.

plotting_fre_mask.ipynb: showing the mask in Fourier domain, compared with the data.

xinv_ir_it1000.npz: an reconstruction result from idr_14.npy (irregular sampling, 1000 iterations for LSQR)

D_all.npy: Multi-source turbulence seismic wavefield (301 shots, 301 receivers)

D_aftmask.npy: D_all.npy after applying mask in space-time domain (for the removal of direct waves and sediment reflection)

RSF.zip: RSF filels for the turbulence seismic wavefield.
