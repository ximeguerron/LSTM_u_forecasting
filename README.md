![image](https://github.com/ximeguerron/LSTM_u_forecasting/assets/16210142/eb35da99-bc46-4e36-9b12-a195ff90268c)<div align="center"><h1>Forecasting the quality of cloud services using an LSTM network</h1></div>

* * *
This repository manages the files used in the experiments of the paper:
_**Forecasting the quality of cloud services using an LSTM network**_
* * *

<p align="center">
    <a href="https://colab.research.google.com/drive/1Fa6seQ6PJU0jgMo7X1jeYzJzK2TmMzJS?usp=sharing">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>
</p>

The following section presents the results obtained for the 16 variables used to develop the experiment, as well as additional information related to them.

These results are:

* Representation of the **_datasets_**  with the observations of 16 QoS metrics extracted from the cloud service SAlert monitoring.
* Model validation metrics consisting of **_RMSE, MAE, MAPE_**
* Model fitting on the training dataset and prediction on the test dataset.

## _Datasets_

| Variable            | Dataset                                                                  |
|---------------------|----------------------------------------------------------------------------|
| Free Memory         | ![FreeMemory_data.jpg](imgs/dataset/FreeMemory_data.jpg)               |
| Used Memory         | ![UsedMemory_data.jpg](imgs/dataset/UsedMemory_data.jpg)               |
| Free Disk           | ![Free Disk_dataset.png](imgs/dataset/FreeDisk_data.jpg)                   |
| Used Disk           | ![Used Disk_dataset.png](imgs/dataset/UsedDisk_data.jpg)                   |
| Disk read/s         | ![Disk read_s_dataset.png](imgs/dataset/Diskreads_data.jpg)               |
| Disk write/s        | ![Disk write_s_dataset.png](imgs/dataset/Diskwrites_data.jpg)             |
| NetBytes In         | ![NetBytes In_dataset.png](imgs/dataset/NetBytesIn_data.jpg)               |
| NetBytes Out        | ![NetBytes Out_dataset.png](imgs/dataset/NetBytesOut_data.jpg)             |
| NetPackets In       | ![NetPackets In_dataset.png](imgs/dataset/NetPacketsIn_data.jpg)           |
| NetPackets Out      |  ![NetPackets Out_dataset.png](imgs/dataset/NetPacketsOut_data.jpg)          |
| Rx packets          | ![Rx packets_dataset.png](imgs/dataset/Rxpackets_data.jpg)                 |
| Tx packets          | ![Tx packets_dataset.png](imgs/dataset/Txpackets_data.jpg)                 |
| CPU percent         | ![MemoryUsedpercent_dataset.png](imgs/dataset/CPUpercent_data.jpg)         |
| Memory Used percent | ![Used Memory_dataset.png](imgs/dataset/MemoryUsedpercent_data.jpg)       |
| Disk Used percent   | ![Disk Used percent_dataset.png](imgs/dataset/DiskUsedpercent_data.jpg) |
| Uptime              | ![Uptime_dataset.png](imgs/dataset/Uptime_data.jpg)                     |

## Metrics

| Variable            | RMSE                                                                     | MAE                                                                     | MAPE                                                                     | 
|---------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **_Free Memory_**        
Iteration 1| ![Free Memory_mrse.png](imgs/LSTM/metrics/fold_0_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/fold_0_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/fold_0_Free%20Memory_mape.png)                   | 
|Iteration 2         | ![Free Memory_mrse.png](imgs/LSTM/metrics/fold_1_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/fold_1_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/fold_1_Free%20Memory_mape.png)                   | 
| Iteration 3        | ![Free Memory_mrse.png](imgs/LSTM/metrics/fold_2_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/fold_2_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/fold_2_Free%20Memory_mape.png)                   | 
| **_Used Memory_**         
Iteration 1| ![Used Memory_rsme.png](imgs/LSTM/metrics/fold_0_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/fold_0_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/LSTM/metrics/fold_0_Used%20Memory_mape.png) | 
| Iteration 2         | ![Used Memory_rsme.png](imgs/LSTM/metrics/fold_1_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/fold_1_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/LSTM/metrics/fold_1_Used%20Memory_mape.png) | 
| Iteration 3         | ![Used Memory_rsme.png](imgs/LSTM/metrics/fold_2_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/fold_2_Used%20Memory_mae.png)   | ![Used Memory_mape.png](imgs/LSTM/metrics/fold_2_Used%20Memory_mape.png)          | 
| **_Free Disk_**           
Iteration 1| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_0_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_0_Freee%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_0_Free%20Disk_mape.png) | 
|Iteration 2| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_1_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_1_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_1_Free%20Disk_mape.png) | 
|Iteration 3| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_2_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_2_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_2_Free%20Disk_mape.png) | 
| **_Used Disk_**           | ![Used Disk_rmse.png](imgs/LSTM/metrics/fold_0_Used%20Disk_rmse.png) | 
 | ![Used Disk_mae.png](imgs/LSTM/metrics/fold_0_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/fold_0_Used%20Disk_mape.png) | 
| Disk read/s         | ![Disk read_s_mrse.png](imgs%2FDisk%20read_s_mrse.png)                   | ![Disk read_s_mae.png](imgs%2FDisk%20read_s_mae.png)                    | ![Disk read_s_mape.png](imgs%2FDisk%20read_s_mape.png)                   | !
| Disk write/s        | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mrse.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mae.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mape.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mase.png)                 |
| NetBytes In         | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mrse.png)                   | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mae.png)                   | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mape.png)                   | 
| NetBytes Out        | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mrse.png)                 | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mae.png)                 | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mape.png)                 | 
| NetPackets In       | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mrse.png)               | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mae.png)               | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mape.png)               | 
| NetPackets Out      |                                                                          |                                                                         |                                                                          |   
| Rx packets          | ![Rx packets_mrse.png](imgs%2FRx%20packets_mrse.png)                     | ![Rx packets_mrse.png](imgs%2FRx%20packets_mae.png)                     | ![Rx packets_mrse.png](imgs%2FRx%20packets_mape.png)                     | 
| Tx packets          | ![Tx packets_mrse.png](imgs%2FTx%20packets_mrse.png)                     | ![Tx packets_mrse.png](imgs%2FTx%20packets_mae.png)                     | ![Tx packets_mrse.png](imgs%2FTx%20packets_mape.png)                     | 
| CPU percent         | ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_0_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_0_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/fold_0_CPU%20percent_mape.png)                   | 
|         | ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_1_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_1_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/fold_1_CPU%20percent_mape.png)                   | 
|         | ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_2_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_2_CPU%20percent_mae.png)                    | ![FCPU percent_mape.png](imgs/LSTM/metrics/fold_2_CPU%20percent_mape.png)  
| Memory Used percent | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mrse.png) | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mae.png) | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mape.png) | 
| Disk Used percent   | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mrse.png)     | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mae.png)     | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mape.png)     | 
| Uptime              | ![Uptime_mrse.png](imgs%2FUptime_mrse.png)                               | ![Uptime_mrse.png](imgs%2FUptime_mae.png)                               | ![Uptime_mrse.png](imgs%2FUptime_mape.png)                               | 

## ARIMA Model Prediction 

| Variable            | Iteration 1                                                                            | Iteration 2                                                                                   | Iteration 3  | 
|---------------------|------------------------------------------------------------------------------------------|--------------------------------------|--------------------------------------------------|
| Free Memory         | ![Free Memory_train_result.png](imgs%2FFree%20Memory_train_result.png)                   | ![Free Memory_test_result.png](imgs%2FFree%20Memory_test_result.png)                   |
| Used Memory         | ![Used Memory_train_result.png](imgs%2FUsed%20Memory_train_result.png)                   | ![Used Memory_test_result.png](imgs%2FUsed%20Memory_test_result.png)                   |
| Free Disk           | ![Free Disk_train_result.png](imgs%2FFree%20Disk_train_result.png)                       | ![Free Disk_test_result.png](imgs%2FFree%20Disk_test_result.png)                       |
| Used Disk           | ![Used Disk_train_result.png](imgs%2FUsed%20Disk_train_result.png)                       | ![Used Disk_test_result.png](imgs%2FUsed%20Disk_test_result.png)                       |
| Disk read/s         | ![Disk read_s_train_result.png](imgs%2FDisk%20read_s_train_result.png)                   | ![Disk read_s_test_result.png](imgs%2FDisk%20read_s_test_result.png)                   |
| Disk write/s        | ![Disk write_s_train_result.png](imgs%2FDisk%20write_s_train_result.png)                 | ![Disk write_s_test_result.png](imgs%2FDisk%20write_s_test_result.png)                 |
| NetBytes In         | ![NetBytes In_train_result.png](imgs%2FNetBytes%20In_train_result.png)                   | ![NetBytes In_test_result.png](imgs%2FNetBytes%20In_test_result.png)                   |
| NetBytes Out        | ![NetBytes Out_train_result.png](imgs%2FNetBytes%20Out_train_result.png)                 | ![NetBytes Out_test_result.png](imgs%2FNetBytes%20Out_test_result.png)                 |
| NetPackets In       | ![NetPackets In_train_result.png](imgs%2FNetPackets%20In_train_result.png)               | ![NetPackets In_test_result.png](imgs%2FNetPackets%20In_test_result.png)               |
| NetPackets Out      |                                                                                          |                                                                                        |
| Rx packets          | ![Rx packets_train_result.png](imgs%2FRx%20packets_train_result.png)                     | ![Rx packets_test_result.png](imgs%2FRx%20packets_test_result.png)                     |
| Tx packets          | ![Tx packets_train_result.png](imgs%2FTx%20packets_train_result.png)                     | ![Tx packets_test_result.png](imgs%2FTx%20packets_test_result.png)                     |
| CPU percent         | ![CPU percent_train_result.png](imgs%2FCPU%20percent_train_result.png)                   | ![CPU percent_test_result.png](imgs%2FCPU%20percent_test_result.png)                   |
| Memory Used percent | ![Memory Used percent_train_result.png](imgs%2FMemory%20Used%20percent_train_result.png) | ![Memory Used percent_test_result.png](imgs%2FMemory%20Used%20percent_test_result.png) |
| Disk Used percent   | ![Disk Used percent_train_result.png](imgs%2FDisk%20Used%20percent_train_result.png)     | ![Disk Used percent_test_result.png](imgs%2FDisk%20Used%20percent_test_result.png)     |
| Uptime              | ![Uptime_train_result.png](imgs%2FUptime_train_result.png)                               | ![Uptime_test_result.png](imgs%2FUptime_test_result.png)                               |


## LSTM Model Results

| Variable            | Training                                                                            | Testing                                                                                |
|---------------------|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| Free Memory         | ![Free Memory_train_result.png](imgs%2FFree%20Memory_train_result.png)                   | ![Free Memory_test_result.png](imgs%2FFree%20Memory_test_result.png)                   |
| Used Memory         | ![Used Memory_train_result.png](imgs%2FUsed%20Memory_train_result.png)                   | ![Used Memory_test_result.png](imgs%2FUsed%20Memory_test_result.png)                   |
| Free Disk           | ![Free Disk_train_result.png](imgs%2FFree%20Disk_train_result.png)                       | ![Free Disk_test_result.png](imgs%2FFree%20Disk_test_result.png)                       |
| Used Disk           | ![Used Disk_train_result.png](imgs%2FUsed%20Disk_train_result.png)                       | ![Used Disk_test_result.png](imgs%2FUsed%20Disk_test_result.png)                       |
| Disk read/s         | ![Disk read_s_train_result.png](imgs%2FDisk%20read_s_train_result.png)                   | ![Disk read_s_test_result.png](imgs%2FDisk%20read_s_test_result.png)                   |
| Disk write/s        | ![Disk write_s_train_result.png](imgs%2FDisk%20write_s_train_result.png)                 | ![Disk write_s_test_result.png](imgs%2FDisk%20write_s_test_result.png)                 |
| NetBytes In         | ![NetBytes In_train_result.png](imgs%2FNetBytes%20In_train_result.png)                   | ![NetBytes In_test_result.png](imgs%2FNetBytes%20In_test_result.png)                   |
| NetBytes Out        | ![NetBytes Out_train_result.png](imgs%2FNetBytes%20Out_train_result.png)                 | ![NetBytes Out_test_result.png](imgs%2FNetBytes%20Out_test_result.png)                 |
| NetPackets In       | ![NetPackets In_train_result.png](imgs%2FNetPackets%20In_train_result.png)               | ![NetPackets In_test_result.png](imgs%2FNetPackets%20In_test_result.png)               |
| NetPackets Out      |                                                                                          |                                                                                        |
| Rx packets          | ![Rx packets_train_result.png](imgs%2FRx%20packets_train_result.png)                     | ![Rx packets_test_result.png](imgs%2FRx%20packets_test_result.png)                     |
| Tx packets          | ![Tx packets_train_result.png](imgs%2FTx%20packets_train_result.png)                     | ![Tx packets_test_result.png](imgs%2FTx%20packets_test_result.png)                     |
| CPU percent         | ![CPU percent_train_result.png](imgs%2FCPU%20percent_train_result.png)                   | ![CPU percent_test_result.png](imgs%2FCPU%20percent_test_result.png)                   |
| Memory Used percent | ![Memory Used percent_train_result.png](imgs%2FMemory%20Used%20percent_train_result.png) | ![Memory Used percent_test_result.png](imgs%2FMemory%20Used%20percent_test_result.png) |
| Disk Used percent   | ![Disk Used percent_train_result.png](imgs%2FDisk%20Used%20percent_train_result.png)     | ![Disk Used percent_test_result.png](imgs%2FDisk%20Used%20percent_test_result.png)     |
| Uptime              | ![Uptime_train_result.png](imgs%2FUptime_train_result.png)                               | ![Uptime_test_result.png](imgs%2FUptime_test_result.png)                               |


