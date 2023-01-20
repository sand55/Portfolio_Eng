# Project: "Steel melting temperature prediction"

In order to optimize production costs, the melallurgicall complex decided to reduce electricity consumption during the steel processing stage. You have to build a model that predicts the temperature of the steel.

The goal of the work is to prepare a model for predicting the optimal steel melting temperature and to prepare a report on the work performed and the selection of the model. Quality metric MAE, on the test sample no more than 7.6, preferably no more than 6.

The target parameter is the temperature from the last measurement of the batch, before sending it to finishing or continuous casting machine.

### Description of the processing step

Steel is processed in a metal ladle with a capacity of about 100 tons. In order for the ladle to withstand high temperatures, it is lined with refractory bricks from the inside. Molten steel is poured into a ladle and heated to the desired temperature with graphite electrodes. They are installed in the lid of the bucket.

Sulfur is removed from the alloy (desulfurization), the chemical composition is corrected by adding impurities, and samples are taken. Steel is alloyed - its composition is changed - by feeding pieces of alloy from a bunker for bulk materials or wire through a special tribe apparatus.

Before introducing alloying additives for the first time, the temperature of the steel is measured and its chemical analysis is carried out. Then the temperature is raised for several minutes, alloying materials are added and the alloy is purged with an inert gas. Then it is stirred and measured again. This cycle is repeated until the target chemical composition and optimum melting temperature are reached.

Then the molten steel is sent to finish the metal or enters the continuous casting machine. From there, the finished product comes out in the form of slab blanks.

### Description of data

The data consists of files obtained from various sources:

- `data_arc.csv` - electrode data;
- `data_bulk.csv` - data on the supply of bulk materials (volume);
- `data_bulk_time.csv` - data on the supply of bulk materials (time);
- `data_gas.csv` - data on alloy gas purge;
- `data_temp.csv` - temperature measurement results;
- `data_wire.csv` - data on wire materials (volume);
- `data_wire_time.csv` - data on wire materials (time).

In all files, the `key` column contains the batch number. There can be several lines in files with the same `key` value: they correspond to different processing iterations.
