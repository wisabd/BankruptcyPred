# BankruptcyPred
Supervised machine learning project (credit to WorldQuant Uni - the project was developed on their virtual machine)


## Dataset (https://archive.ics.uci.edu/dataset/365/polish+companies+bankruptcy+data)
It is contained in a file called poland-bankruptcy-data-2009.json. It is in a dictionary format with keys data, metadata, schema. Associated with the key data are the values of company id, 64 featues and a True/False label for bankruptcy.


| Feature   | Description                                                                                   |
|-----------|-----------------------------------------------------------------------------------------------|
| feat_1    | net profit / total assets                                                                     |
| feat_2    | total liabilities / total assets                                                              |
| feat_3    | working capital / total assets                                                                |
| feat_4    | current assets / short-term liabilities                                                       |
| feat_5    | [(cash + short-term securities + receivables - short-term liabilities) / (operating expenses - depreciation)] * 365 |
| feat_6    | retained earnings / total assets                                                              |
| feat_7    | EBIT / total assets                                                                           |
| feat_8    | book value of equity / total liabilities                                                      |
| feat_9    | sales / total assets                                                                          |
| feat_10   | equity / total assets                                                                         |
| feat_11   | (gross profit + extraordinary items + financial expenses) / total assets                     |
| feat_12   | gross profit / short-term liabilities                                                         |
| feat_13   | (gross profit + depreciation) / sales                                                         |
| feat_14   | (gross profit + interest) / total assets                                                      |
| feat_15   | (total liabilities * 365) / (gross profit + depreciation)                                     |
| feat_16   | (gross profit + depreciation) / total liabilities                                             |
| feat_17   | total assets / total liabilities                                                              |
| feat_18   | gross profit / total assets                                                                   |
| feat_19   | gross profit / sales                                                                          |
| feat_20   | (inventory * 365) / sales                                                                     |
| feat_21   | sales (n) / sales (n-1)                                                                       |
| feat_22   | profit on operating activities / total assets                                                 |
| feat_23   | net profit / sales                                                                            |
| feat_24   | gross profit (in 3 years) / total assets                                                      |
| feat_25   | (equity - share capital) / total assets                                                       |
| feat_26   | (net profit + depreciation) / total liabilities                                               |
| feat_27   | profit on operating activities / financial expenses                                           |
| feat_28   | working capital / fixed assets                                                                |
| feat_29   | logarithm of total assets                                                                     |
| feat_30   | (total liabilities - cash) / sales                                                            |
| feat_31   | (gross profit + interest) / sales                                                             |
| feat_32   | (current liabilities * 365) / cost of products sold                                           |
| feat_33   | operating expenses / short-term liabilities                                                   |
| feat_34   | operating expenses / total liabilities                                                        |
| feat_35   | profit on sales / total assets                                                                |
| feat_36   | total sales / total assets                                                                    |
| feat_37   | (current assets - inventories) / long-term liabilities                                        |
| feat_38   | constant capital / total assets                                                               |
| feat_39   | profit on sales / sales                                                                       |
| feat_40   | (current assets - inventory - receivables) / short-term liabilities                           |
| feat_41   | total liabilities / ((profit on operating activities + depreciation) * (12/365))             |
| feat_42   | profit on operating activities / sales                                                        |
| feat_43   | rotation receivables + inventory turnover in days                                             |
| feat_44   | (receivables * 365) / sales                                                                   |
| feat_45   | net profit / inventory                                                                        |
| feat_46   | (current assets - inventory) / short-term liabilities                                         |
| feat_47   | (inventory * 365) / cost of products sold                                                     |
| feat_48   | EBITDA (profit on operating activities - depreciation) / total assets                         |
| feat_49   | EBITDA (profit on operating activities - depreciation) / sales                                |
| feat_50   | current assets / total liabilities                                                            |
| feat_51   | short-term liabilities / total assets                                                         |
| feat_52   | (short-term liabilities * 365) / cost of products sold)                                       |
| feat_53   | equity / fixed assets                                                                         |
| feat_54   | constant capital / fixed assets                                                               |
| feat_55   | working capital                                                                               |
| feat_56   | (sales - cost of products sold) / sales                                                       |
| feat_57   | (current assets - inventory - short-term liabilities) / (sales - gross profit - depreciation) |
| feat_58   | total costs / total sales                                                                     |
| feat_59   | long-term liabilities / equity                                                                |
| feat_60   | sales / inventory                                                                             |
| feat_61   | sales / receivables                                                                           |
| feat_62   | (short-term liabilities * 365) / sales                                                        |
| feat_63   | sales / short-term liabilities                                                                |
| feat_64   | sales / fixed assets                                                                          |
| bankrupt  | Whether company went bankrupt at end of forecasting period (2013)                             |















## Citation (Original Paper)

Ziȩba, Maciej et al. “Ensemble boosted trees with synthetic features generation in application to bankruptcy prediction.” Expert Syst. Appl. 58 (2016): 93-101.
