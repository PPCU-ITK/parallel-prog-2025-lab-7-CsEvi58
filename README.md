[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/2CuuzvUr)
# assignment-7
module load nvhpc
module load craype-accel-nvidia80
nvc++ -mp=gpu -gpu=cc80 -Ofast laplace2d.cpp -o laplace -Minfo=accel,mp
srun -p gpu --gres=gpu:1 --ntasks=1 --time=00:05:00 --mem=40G --reservation=p_es_itkpp_204 ./laplace


Step 0 completed, total kinetic energy: 9825.76
Step 50 completed, total kinetic energy: 9595.83
Step 100 completed, total kinetic energy: 9419.26
Step 150 completed, total kinetic energy: 9254.27
Step 200 completed, total kinetic energy: 9096.12
Step 250 completed, total kinetic energy: 8941.93
Step 300 completed, total kinetic energy: 8789.82
Step 350 completed, total kinetic energy: 8638.8
Step 400 completed, total kinetic energy: 8488.7
Step 450 completed, total kinetic energy: 8340.5
Step 500 completed, total kinetic energy: 8200.49
Step 550 completed, total kinetic energy: 8084
Step 600 completed, total kinetic energy: 8004.93
Step 650 completed, total kinetic energy: 7962.46
Step 700 completed, total kinetic energy: 7943.53
Step 750 completed, total kinetic energy: 7933.54
Step 800 completed, total kinetic energy: 7923.31
Step 850 completed, total kinetic energy: 7909.65
Step 900 completed, total kinetic energy: 7892.89
Step 950 completed, total kinetic energy: 7874.44
Step 1000 completed, total kinetic energy: 7855.53
Step 1050 completed, total kinetic energy: 7836.97
Step 1100 completed, total kinetic energy: 7819.23
Step 1150 completed, total kinetic energy: 7802.63
Step 1200 completed, total kinetic energy: 7787.42
Step 1250 completed, total kinetic energy: 7773.83
Step 1300 completed, total kinetic energy: 7762.06
Step 1350 completed, total kinetic energy: 7752.25
Step 1400 completed, total kinetic energy: 7744.47
Step 1450 completed, total kinetic energy: 7738.68
Step 1500 completed, total kinetic energy: 7734.74
Step 1550 completed, total kinetic energy: 7732.46
Step 1600 completed, total kinetic energy: 7731.59
Step 1650 completed, total kinetic energy: 7731.88
Step 1700 completed, total kinetic energy: 7733.08
Step 1750 completed, total kinetic energy: 7734.95
Step 1800 completed, total kinetic energy: 7737.31
Step 1850 completed, total kinetic energy: 7739.97
Step 1900 completed, total kinetic energy: 7742.83
Step 1950 completed, total kinetic energy: 7745.78
Simulation time: 0.229495 seconds