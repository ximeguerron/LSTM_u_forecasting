<h1>Forecasting the quality of cloud services using an LSTM network</h1></div>

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

## Index
1. [Dataset](#datos)
2. [LSTM Accuracy Metrics](#Metric)
3. [ARIMA model predictions](#ARIMA)
4. [LSTM model predictions](#LSTM)


## _Datasets_ {#Datos}
Representation of the **_datasets_**  with the observations of 16 QoS metrics extracted from the cloud service SAlert monitoring.

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

## LSTM Accuracy Metrics {#Metric}
LSTM model performance evaluation using accuracy metrics **_RMSE, MAE, MAPE_** 

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
Iteration 1| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_0_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_0_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_0_Free%20Disk_mape.png) | 
|Iteration 2| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_1_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_1_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_1_Free%20Disk_mape.png) | 
|Iteration 3| ![FreeDisk_rsme.png](imgs/LSTM/metrics/fold_2_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/fold_2_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/fold_2_Free%20Disk_mape.png) | 
| **_Used Disk_**
Iteration 1| ![Used Disk_rmse.png](imgs/LSTM/metrics/fold_0_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/fold_0_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/fold_0_Used%20Disk_mape.png) | 
|Iteration 2| ![Used Disk_rmse.png](imgs/LSTM/metrics/fold_1_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/fold_1_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/fold_1_Used%20Disk_mape.png) | 
|Iteration 3| ![Used Disk_rmse.png](imgs/LSTM/metrics/fold_2_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/fold_2_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/fold_2_Used%20Disk_mape.png) | 
| **_Disk read/s_**
Iteration 1|![Disk_read_s_rmse.png](imgs/LSTM/metrics/fold_0_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/fold_0_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/fold_0_Disk%20read_s_mape.png) | 
|Iteration 2|![Disk_read_s_rmse.png](imgs/LSTM/metrics/fold_1_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/fold_1_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/fold_1_Disk%20read_s_mape.png) | 
|Iteration 3|![Disk_read_s_rmse.png](imgs/LSTM/metrics/fold_2_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/fold_2_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/fold_2_Disk%20read_s_mape.png) | 
| **_Disk write/s_**
Iteration 1|![Disk write_s_rmse.png](imgs/LSTM/metrics/fold_0_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/fold_0_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/fold_0_Disk%20write_s_mape.png) | 
|Iteration 2|![Disk write_s_rmse.png](imgs/LSTM/metrics/fold_1_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/fold_1_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/fold_1_Disk%20write_s_mape.png) | 
|Iteration 3|![Disk write_s_rmse.png](imgs/LSTM/metrics/fold_2_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/fold_2_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/fold_2_Disk%20write_s_mape.png) | 
| **_NetBytes In_**     
Iteration 1| ![NetBytes In_rmse.png](imgs/LSTM/metrics/fold_0_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/fold_0_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/fold_0_NetBytes%20In_mape.png) | 
|Iteration 2| ![NetBytes In_rmse.png](imgs/LSTM/metrics/fold_1_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/fold_1_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/fold_1_NetBytes%20In_mape.png) | 
|Iteration 3| ![NetBytes In_rmse.png](imgs/LSTM/metrics/fold_2_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/fold_2_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/fold_2_NetBytes%20In_mape.png) | 
| **_NetBytes Out_**  
Iteration 1 |![NetBytes Out_rmse.png](imgs/LSTM/metrics/fold_0_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/fold_0_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/fold_0_NetBytes%20Out_mape.png) | 
|Iteration 2 | ![NetBytes Out_rmse.png](imgs/LSTM/metrics/fold_1_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/fold_1_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/fold_1_NetBytes%20Out_mape.png) |
|Iteration 3 | ![NetBytes Out_rmse.png](imgs/LSTM/metrics/fold_2_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/fold_2_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/fold_2_NetBytes%20Out_mape.png) |
| **_NetPackets In_**   
Iteration 1| ![NetPackets In_rmse.png](imgs/LSTM/metrics/fold_0_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/fold_0_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/fold_0_NetPackets%20In_mape.png) | 
|Iteration 2| ![NetPackets In_rmse.png](imgs/LSTM/metrics/fold_1_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/fold_1_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/fold_1_NetPackets%20In_mape.png) | 
|Iteration 3| ![NetPackets In_rmse.png](imgs/LSTM/metrics/fold_2_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/fold_2_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/fold_2_NetPackets%20In_mape.png) | 
| **_NetPackets Out_**   
Iteration 1|![NetPackets Out_rmse.png](imgs/LSTM/metrics/fold_0_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/fold_0_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/fold_0_NetPackets%20Out_mape.png) | 
|Iteration 2|![NetPackets Out_rmse.png](imgs/LSTM/metrics/fold_1_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/fold_1_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/fold_1_NetPackets%20Out_mape.png) | 
| Iteration 3|![NetPackets Out_rmse.png](imgs/LSTM/metrics/fold_2_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/fold_2_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/fold_2_NetPackets%20Out_mape.png) |              
| **_Rx packets_**    
Iteration 1|![Rx packets_rmse.png](imgs/LSTM/metrics/fold_0_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/fold_0_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/fold_0_Rx%20packets_mape.png) | 
|Iteration 2|![Rx packets_rmse.png](imgs/LSTM/metrics/fold_1_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/fold_1_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/fold_1_Rx%20packets_mape.png) | 
|Iteration 3|![Rx packets_rmse.png](imgs/LSTM/metrics/fold_2_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/fold_2_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/fold_2_Rx%20packets_mape.png) | 
| **_Tx packets_**         
Iteration 1 |![Tx packets_rmse.png](imgs/LSTM/metrics/fold_0_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/fold_0_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/fold_0_Tx%20packets_mape.png) | 
|Iteration 2 |![Tx packets_rmse.png](imgs/LSTM/metrics/fold_1_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/fold_1_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/fold_1_Tx%20packets_mape.png) | 
|Iteration 3 |![Tx packets_rmse.png](imgs/LSTM/metrics/fold_2_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/fold_2_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/fold_2_Tx%20packets_mape.png) | 
| **_CPU percent_**
Iteration 1| ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_0_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_0_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/fold_0_CPU%20percent_mape.png) | 
|Iteration 2         | ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_1_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_1_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/fold_1_CPU%20percent_mape.png) | 
| Iteration 3| ![CPU percent_mrse.png](imgs/LSTM/metrics/fold_2_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/fold_2_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/fold_2_CPU%20percent_mape.png)  
| **_Memory Used percent_** 
Iteration 1 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/fold_0_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/fold_0_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/fold_0_Memory%20Used%20percent_mape.png) | 
|Iteration 2 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/fold_1_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/fold_1_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/fold_1_Memory%20Used%20percent_mape.png) |
|Iteration 3 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/fold_2_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/fold_2_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/fold_2_Memory%20Used%20percent_mape.png) |
| **_Disk Used percent_**  
Iteration 1 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/fold_0_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/fold_0_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/fold_0_Disk%20Used%20percent_mape.png) | 
Iteration 2 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/fold_1_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/fold_1_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/fold_1_Disk%20Used%20percent_mape.png) |
Iteration 3 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/fold_2_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/fold_2_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/fold_2_Disk%20Used%20percent_mape.png) |
| **_Uptime_**
Iteration 1 | ![Uptime_rmse.png](imgs/LSTM/metrics/fold_0_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/fold_0_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/fold_0_Uptime_mape.png) | 
|Iteration 2 |  ![Uptime_rmse.png](imgs/LSTM/metrics/fold_1_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/fold_1_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/fold_1_Uptime_mape.png) | 
|Iteration 3 |  ![Uptime_rmse.png](imgs/LSTM/metrics/fold_2_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/fold_2_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/fold_2_Uptime_mape.png) | 

## ARIMA Model Prediction {#ARIMA}
ARIMA Model fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         | ![FreeMemory_.png](imgs/Arima/fold-0_FreeMemory_test_result.jpg) | 	![FreeMemory_.png](imgs/Arima/fold-1_FreeMemory_test_result.jpg) | 	![FreeMemory_.png](imgs/Arima/fold-2_FreeMemory_test_result.jpg) | 
| Used Memory         | ![UsedMemory_.png](imgs/Arima/fold-0_UsedMemory_test_result.jpg) | 	![UsedMemory_.png](imgs/Arima/fold-1_UsedMemory_test_result.jpg) | 	![UsedMemory_.png](imgs/Arima/fold-2_UsedMemory_test_result.jpg) |   
| Free Disk           | ![FreeDisk_test.png](imgs/Arima/fold-0_FreeDisk_test_result.jpg) | 	![FreeDisk_test.png](imgs/Arima/fold-1_FreeDisk_test_result.jpg) | 	![FreeDisk_test.png](imgs/Arima/fold-2_FreeDisk_test_result.jpg) | 
| Used Disk           | ![UsedDisk_test.png](imgs/Arima/fold-0_UsedDisk_test_result.jpg) | 	![UsedDisk_test.png](imgs/Arima/fold-1_UsedDisk_test_result.jpg) | 	![UsedDisk_test.png](imgs/Arima/fold-2_UsedDisk_test_result.jpg) | 
| Disk read/s         | ![Diskreads_test.png](imgs/Arima/fold-0_Diskreads_test_result.jpg) | 	![Diskreads_test.png](imgs/Arima/fold-1_Diskreads_test_result.jpg) | 	![Diskreads_test.png](imgs/Arima/fold-2_Diskreads_test_result.jpg) | 
| Disk write/s        | ![Diskwrites_test.png](imgs/Arima/fold-0_Diskwrites_test_result.jpg) | 	![Diskwrites_test.png](imgs/Arima/fold-1_Diskwrites_test_result.jpg) | 	![Diskwrites_test.png](imgs/Arima/fold-2_Diskwrites_test_result.jpg) | 
| NetBytes In         | ![NetBytes In_test.png](imgs/Arima/fold-0_NetBytesIn_test_result.jpg) | 	![NetBytes In_test.png](imgs/Arima/fold-1_NetBytesIn_test_result.jpg) | 	![NetBytes In_test.png](imgs/Arima/fold-2_NetBytesIn_test_result.jpg) | 
| NetBytes Out        | ![NetBytesOut_test.png](imgs/Arima/fold-0_NetBytesOut_test_result.jpg) | 	![NetBytesOut_test.png](imgs/Arima/fold-1_NetBytesOut_test_result.jpg) | 	![NetBytesOut_test.png](imgs/Arima/fold-2_NetBytesOut_test_result.jpg) | 
| NetPackets In       | ![NetPacketsIn_test.png](imgs/Arima/fold-0_NetPacketsIn_test_result.jpg) | 	![NetPacketsIn_test.png](imgs/Arima/fold-1_NetPacketsIn_test_result.jpg) | 	![NetPacketsIn_test.png](imgs/Arima/fold-2_NetPacketsIn_test_result.jpg) | 
| NetPackets Out      |  ![NetPacketsOut_test.png](imgs/Arima/fold-0_NetPacketsOut_test_result.jpg) | 	![NetPacketsOut_test.png](imgs/Arima/fold-1_NetPacketsOut_test_result.jpg) | 	![NetPacketsOut_test.png](imgs/Arima/fold-2_NetPacketsOut_test_result.jpg) |
| Rx packets          | ![Rxpackets_test.png](imgs/Arima/fold-0_Rxpackets_test_result.jpg) | 	![Rxpackets_test.png](imgs/Arima/fold-1_Rxpackets_test_result.jpg) | 	![Rxpackets_test.png](imgs/Arima/fold-2_Rxpackets_test_result.jpg) | 
| Tx packets          | ![Txpackets_test.png](imgs/Arima/fold-0_Txpackets_test_result.jpg) | 	![Txpackets_test.png](imgs/Arima/fold-1_Txpackets_test_result.jpg) | 	![Txpackets_test.png](imgs/Arima/fold-2_Txpackets_test_result.jpg) | 
| CPU percent         | ![CPUpercent_test.png](imgs/Arima/fold-0_CPUpercent_test_result.jpg) | 	![CPUpercent_test.png](imgs/Arima/fold-1_CPUpercent_test_result.jpg) | 	![CPUpercent_test.png](imgs/Arima/fold-2_CPUpercent_test_result.jpg) | 
| Memory Used percent | ![MemoryUsedpercent_test.png](imgs/Arima/fold-0_MemoryUsedpercent_test_result.jpg) | 	![MemoryUsedpercent_test.png](imgs/Arima/fold-1_MemoryUsedpercent_test_result.jpg) | 	![MemoryUsedpercent_test.png](imgs/Arima/fold-2_MemoryUsedpercent_test_result.jpg) | 
| Disk Used percent   | ![DiskUsedpercent_test.png](imgs/Arima/fold-0_DiskUsedpercent_test_result.jpg) | 	![DiskUsedpercent_test.png](imgs/Arima/fold-1_DiskUsedpercent_test_result.jpg) | 	![DiskUsedpercent_test.png](imgs/Arima/fold-2_DiskUsedpercent_test_result.jpg) | 
| Uptime              |![Uptime_rmse.png](imgs/Arima/fold-0_Uptime_test_result.jpg) | 	![Uptime_mae.png](imgs/Arima/fold-1_Uptime_test_result.jpg) | 	![Uptime_mape.png](imgs/Arima/fold-2_Uptime_test_result.jpg) | 



## LSTM Model Prediction {#LSTM}
LSTM Model fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         |![Free Memory_test.png](imgs/LSTM/results/fold_0_Free%20Memory_train_result.png) | 	![Free Memory_test.png](imgs/LSTM/results/fold_1_Free%20Memory_train_result.png) | 	![Free Memory_test.png](imgs/LSTM/results/fold_2_Free%20Memory_train_result.png)| 
| Used Memory         | ![Used Memory_test.png](imgs/LSTM/results/fold_0_Used%20Memory_train_result.png) | 	![Used Memory_test.png](imgs/LSTM/results/fold_1_Used%20Memory_train_result.png) | 	![Used Memory_test.png](imgs/LSTM/results/fold_2_Used%20Memory_train_result.png)|
| Free Disk           | ![Free Disk_test.png](imgs/LSTM/results/fold_0_Free%20Disk_train_result.png) | 	![Free Disk_test.png](imgs/LSTM/results/fold_1_Free%20Disk_train_result.png) | 	![Free Disk_test.png](imgs/LSTM/results/fold_2_Free%20Disk_train_result.png) |  
| Used Disk           | ![Used Disk_test.png](imgs/LSTM/results/fold_0_Used%20Disk_train_result.png) | 	![Used Disk_test.png](imgs/LSTM/results/fold_1_Used%20Disk_train_result.png) | 	![Used Disk_test.png](imgs/LSTM/results/fold_2_Used%20Disk_train_result.png) | 
| Disk read/s         | ![Disk read_s_test.png](imgs/LSTM/results/fold_0_Disk%20read_s_train_result.png) | 	![Disk read_s_test.png](imgs/LSTM/results/fold_1_Disk%20read_s_train_result.png) | 	![Disk read_s_test.png](imgs/LSTM/results/fold_2_Disk%20read_s_train_result.png) | 
| Disk write/s        | ![Disk write_s_test.png](imgs/LSTM/results/fold_0_Disk%20write_s_train_result.png) | 	![Disk write_s_test.png](imgs/LSTM/results/fold_1_Disk%20write_s_train_result.png) | 	![Disk write_s_test.png](imgs/LSTM/results/fold_2_Disk%20write_s_train_result.png) | 
| NetBytes In   | ![NetBytes In_test.png](imgs/LSTM/results/fold_0_NetBytes%20In_train_result.png) | 	![NetBytes In_test.png](imgs/LSTM/results/fold_1_NetBytes%20In_train_result.png) | 	![NetBytes In_test.png](imgs/LSTM/results/fold_2_NetBytes%20In_train_result.png)| 
| NetBytes Out        | ![NetBytes Out_test.png](imgs/LSTM/results/fold_0_NetBytes%20Out_train_result.png) | 	![NetBytes Out_test.png](imgs/LSTM/results/fold_1_NetBytes%20Out_train_result.png) | 	![NetBytes Out_test.png](imgs/LSTM/results/fold_2_NetBytes%20Out_train_result.png) | 
| NetPackets In       | ![NetPackets In_test.png](imgs/LSTM/results/fold_0_NetPackets%20In_train_result.png) | 	![NetPackets In_test.png](imgs/LSTM/results/fold_1_NetPackets%20In_train_result.png) | 	![NetPackets In_test.png](imgs/LSTM/results/fold_2_NetPackets%20In_train_result.png) |
| NetPackets Out      |   ![NetPackets Out_test.png](imgs/LSTM/results/fold_0_NetPackets%20Out_train_result.png) | 	![NetPackets Out_test.png](imgs/LSTM/results/fold_1_NetPackets%20Out_train_result.png) | 	![NetPackets Out_test.png](imgs/LSTM/results/fold_2_NetPackets%20Out_train_result.png) | 
| Rx packets          | ![Rx packets_test.png](imgs/LSTM/results/fold_0_Rx%20packets_train_result.png) | 	![Rx packets_test.png](imgs/LSTM/results/fold_1_Rx%20packets_train_result.png) | 	![Rx packets_test.png](imgs/LSTM/results/fold_2_Rx%20packets_train_result.png) | 
| Tx packets          | ![Tx packets_test.png](imgs/LSTM/results/fold_0_Tx%20packets_train_result.png) | 	![Tx packets_test.png](imgs/LSTM/results/fold_1_Tx%20packets_train_result.png) | 	![Tx packets_test.png](imgs/LSTM/results/fold_2_Tx%20packets_train_result.png) | 
| CPU percent         | ![CPU percent_test.png](imgs/LSTM/results/fold_0_CPU%20percent_train_result.png) | 	![CPU percent_test.png](imgs/LSTM/results/fold_1_CPU%20percent_train_result.png) | 	![CPU percent_test.png](imgs/LSTM/results/fold_2_CPU%20percent_train_result.png)| 
| Memory Used percent | ![Memory Used percent_test.png](imgs/LSTM/results/fold_0_Memory%20Used%20percent_train_result.png) | 	![Memory Used percent_test.png](imgs/LSTM/results/fold_1_Memory%20Used%20percent_train_result.png) | 	![Memory Used percent_test.png](imgs/LSTM/results/fold_2_Memory%20Used%20percent_train_result.png) | 
| Disk Used percent   | ![Disk Used percent_test.png](imgs/LSTM/results/fold_0_Disk%20Used%20percent_train_result.png) | 	![Disk Used percent_test.png](imgs/LSTM/results/fold_1_Disk%20Used%20percent_train_result.png) | 	![Disk Used percent_test.png](imgs/LSTM/results/fold_2_Disk%20Used%20percent_train_result.png) | 
| Uptime              | ![Uptime_test.png](imgs/LSTM/results/fold_0_Uptime_train_result.png) | 	![Uptime_test.png](imgs/LSTM/results/fold_1_Uptime_train_result.png) | 	![Uptime_test.png](imgs/LSTM/results/fold_2_Uptime_train_result.png) | 


