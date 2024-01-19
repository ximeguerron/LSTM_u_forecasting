<div align="center"><h1>Forecasting the quality of cloud services using an LSTM network</h1></div>

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

* Representation of the **_training, validation and test_** datasets with the observations extracted from the cloud service SAlert monitoring.
* Model validation metrics consisting of **_RMSE, MAE, MAPE, MASE_**
* Model fitting on the training dataset and prediction on the test dataset.

## _Datasets_

| Variable            | Dataset                                                                  |
|---------------------|----------------------------------------------------------------------------|
| Free Memory         | ![Free Memory_dataset.png](imgs%2FFree%20Memory_dataset.png)               |
| Used Memory         | ![Used Memory_dataset.png](imgs%2FUsed%20Memory_dataset.png)               |
| Free Disk           | ![Free Disk_dataset.png](imgs%2FFree%20Disk_dataset.png)                   |
| Used Disk           | ![Used Disk_dataset.png](imgs%2FUsed%20Disk_dataset.png)                   |
| Disk read/s         | ![Disk read_s_dataset.png](imgs%2FDisk%20read_s_dataset.png)               |
| Disk write/s        | ![Disk write_s_dataset.png](imgs%2FDisk%20write_s_dataset.png)             |
| NetBytes In         | ![NetBytes In_dataset.png](imgs%2FNetBytes%20In_dataset.png)               |
| NetBytes Out        | ![NetBytes Out_dataset.png](imgs%2FNetBytes%20Out_dataset.png)             |
| NetPackets In       | ![NetPackets In_dataset.png](imgs%2FNetPackets%20In_dataset.png)           |
| NetPackets Out      |                                                                            |
| Rx packets          | ![Rx packets_dataset.png](imgs%2FRx%20packets_dataset.png)                 |
| Tx packets          | ![Tx packets_dataset.png](imgs%2FTx%20packets_dataset.png)                 |
| CPU percent         | ![Uptime_dataset.png](imgs%2FUptime_dataset.png)                           |
| Memory Used percent | ![Used Memory_dataset.png](imgs%2FUsed%20Memory_dataset.png)               |
| Disk Used percent   | ![Disk Used percent_dataset.png](imgs%2FDisk%20Used%20percent_dataset.png) |
| Uptime              | ![Uptime_dataset.png](imgs%2FUptime_dataset.png)                           |

## Metrics

| Variable            | RMSE                                                                     | MAE                                                                     | MAPE                                                                     | MASE                                                                     |
|---------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------|--------------------------------------------------------------------------|
| Free Memory         | ![Free Memory_mrse.png](imgs%2FFree%20Memory_mrse.png)                   | ![Free Memory_mae.png](imgs%2FFree%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs%2FFree%20Memory_mape.png)                   | ![Free Memory_mase.png](imgs%2FFree%20Memory_mase.png)                   |
| Used Memory         | ![Used Memory_rsme.png](imgs%2FUsed%20Memory_rsme.png)                   | ![Used Memory_mae.png](imgs%2FUsed%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs%2FUsed%20Memory_mape.png)                   | ![Used Memory_mase.png](imgs%2FUsed%20Memory_mase.png)                   |
| Free Disk           | ![Free Disk_mrse.png](imgs%2FFree%20Disk_mrse.png)                       | ![Free Disk_mae.png](imgs%2FFree%20Disk_mae.png)                        | ![Free Disk_mase.png](imgs%2FFree%20Disk_mape.png)                       | ![Free Disk_mase.png](imgs%2FFree%20Disk_mase.png)                       |
| Used Disk           | ![Used Disk_mrse.png](imgs%2FUsed%20Disk_mrse.png)                       | ![Used Disk_mae.png](imgs%2FUsed%20Disk_mae.png)                        | ![Used Disk_mape.png](imgs%2FUsed%20Disk_mape.png)                       | ![Used Disk_mase.png](imgs%2FUsed%20Disk_mase.png)                       |
| Disk read/s         | ![Disk read_s_mrse.png](imgs%2FDisk%20read_s_mrse.png)                   | ![Disk read_s_mae.png](imgs%2FDisk%20read_s_mae.png)                    | ![Disk read_s_mape.png](imgs%2FDisk%20read_s_mape.png)                   | ![Disk read_s_mase.png](imgs%2FDisk%20read_s_mase.png)                   |
| Disk write/s        | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mrse.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mae.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mape.png)                 | ![Disk write_s_mrse.png](imgs%2FDisk%20write_s_mase.png)                 |
| NetBytes In         | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mrse.png)                   | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mae.png)                   | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mape.png)                   | ![NetBytes In_mrse.png](imgs%2FNetBytes%20In_mase.png)                   |
| NetBytes Out        | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mrse.png)                 | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mae.png)                 | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mape.png)                 | ![NetBytes Out_mrse.png](imgs%2FNetBytes%20Out_mase.png)                 |
| NetPackets In       | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mrse.png)               | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mae.png)               | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mape.png)               | ![NetPackets In_mrse.png](imgs%2FNetPackets%20In_mase.png)               |
| NetPackets Out      |                                                                          |                                                                         |                                                                          |                                                                          |
| Rx packets          | ![Rx packets_mrse.png](imgs%2FRx%20packets_mrse.png)                     | ![Rx packets_mrse.png](imgs%2FRx%20packets_mae.png)                     | ![Rx packets_mrse.png](imgs%2FRx%20packets_mape.png)                     | ![Rx packets_mrse.png](imgs%2FRx%20packets_mase.png)                     |
| Tx packets          | ![Tx packets_mrse.png](imgs%2FTx%20packets_mrse.png)                     | ![Tx packets_mrse.png](imgs%2FTx%20packets_mae.png)                     | ![Tx packets_mrse.png](imgs%2FTx%20packets_mape.png)                     | ![Tx packets_mrse.png](imgs%2FTx%20packets_mase.png)                     |
| CPU percent         | ![CPU percent_mrse.png](imgs%2FCPU%20percent_mrse.png)                   | ![CPU percent_mrse.png](imgs%2FCPU%20percent_mae.png)                   | ![CPU percent_mrse.png](imgs%2FCPU%20percent_mape.png)                   | ![CPU percent_mrse.png](imgs%2FCPU%20percent_mase.png)                   |
| Memory Used percent | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mrse.png) | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mae.png) | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mape.png) | ![Memory Used percent_mrse.png](imgs%2FMemory%20Used%20percent_mase.png) |
| Disk Used percent   | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mrse.png)     | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mae.png)     | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mape.png)     | ![Disk Used percent_mrse.png](imgs%2FDisk%20Used%20percent_mase.png)     |
| Uptime              | ![Uptime_mrse.png](imgs%2FUptime_mrse.png)                               | ![Uptime_mrse.png](imgs%2FUptime_mae.png)                               | ![Uptime_mrse.png](imgs%2FUptime_mape.png)                               | ![Uptime_mrse.png](imgs%2FUptime_mase.png)                               |

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


