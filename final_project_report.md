# Final Project

## Question One

### Datasets

- Nike Manufacturing
- Current classification by income (World Development Indicators - The World Bank)

### Data Preparation

Clean both Nike Manufacturing and World Bank Income Group. In the Nike dataset, converted the data types for columns, `% Female Workers` & `% Migrant Workerss`, from `chr` to `dbl`.

In the World Bank dataset, only the `List of economies` is used. The following columns are dropped: `Code`, `Region`, `Lending category`, `Column1`. Last the last rows that represent the summary of the dataset is dropped.

Last the datasets are merge by using a left join on `Country/Region` == `Country.Region`.

## Question Three

### Data Preparation

Create two new columns: `Number of female workers` (`Total Workers` multiplied by the `% Female Workers`) & `Number of male workers` (`Total Workers` minus `Number of female workers`)

### Data Processing

Two sample T-test using count number of both male and female workers.

### Inference

The p-value is $0.2995$ which is bigger than $0.05$. It failed to reject the null hypothesis that mean of female workers is equal to the mean of male workers.