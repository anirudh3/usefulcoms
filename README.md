# usefulcoms
Just some useful life saving commands


### remote Jupyter

jupyter notebook --no-browser --port=8889

ssh -N -L localhost:8888:localhost:8889 user@remote_host


### @ Abridge

copying files locally:
_path_from = "/home/all_stm_all/presidio_stm_0/"
_path_to = "/home//test_set_6k"
for fi in tqdm(test_files_all):
    _cmd = "cp " + _path_from + fi + ".stm " + _path_to
    os.system(_cmd)
    
copying one instance to another:
gcloud compute copy-files src dest
gcloud compute copy-files -r src_folder dest

