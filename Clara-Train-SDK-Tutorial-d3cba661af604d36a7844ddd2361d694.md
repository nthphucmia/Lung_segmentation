# Clara Train SDK Tutorial

# 1. Prerequiste

- docker-compose version 1.29
- docker engine
- cuda nvidia drivers

## 2. Install Clara SDK and start AIAA server

- Download folder scripts in this repo:

    [https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts](https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts)

- Pull and Run Clara v4:

Pull and Run container Clara v4 by using script:

[https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/startDocker.sh](https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/startDocker.sh)

```

cd scripts
sudo installDocker.sh
```

- Pull and Start the latest clara train SDK and Triton server for AIAA.

[https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/docker-compose.yml](https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/docker-compose.yml)

```
cd scripts
./startClaraTrainNoteBooks.sh
```

You also can customize docker compose in file docker-compose.yml:

[https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/docker-compose.yml](https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/scripts/docker-compose.yml)

```
ports:
  - "3030:8888"  # Jupyter lab port
  - "3031:5000"  # AIAA port
```

- Go to browser with url '"127.0.0.1:3030" and use token:

token=3e5ef35f982ea5a3e432322b07b6d33b5fc51a4fcb0ffa88

# 3. Load Model to AIAA Server

link : [https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/AIAA/AIAA.ipynb](https://github.com/NVIDIA/clara-train-examples/blob/master/PyTorch/NoteBooks/AIAA/AIAA.ipynb)

1 ⇒ 3.2 

# 4. 3D Slicer Plugin