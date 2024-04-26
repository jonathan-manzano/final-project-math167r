# Final Project

## Question One

### Datasets

- Nike Manufacturing
- Current classification by income (World Development Indicators - The World Bank)

### Data Preparation

Clean both Nike Manufacturing and World Bank Income Group. In the Nike dataset, converted the data types for columns, `% Female Workers` & `% Migrant Workerss`, from `chr` to `dbl`.

In the World Bank dataset, only the `List of economies` is used. The following columns are dropped: `Code`, `Region`, `Lending category`, `Column1`. Last the last rows that represent the summary of the dataset is dropped.

Last the datasets are merge by using a left join on `Country/Region` == `Country.Region`.
