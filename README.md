# evaluate-parquet-over-csv
import pandas as pd
df = pd.read_csv('/content/prices.csv')
df.head()
<img width="862" alt="Screen Shot 2022-09-13 at 10 06 39" src="https://user-images.githubusercontent.com/5858494/189798677-625d8118-93df-40c9-9510-cb344dfaea47.png">

df.to_parquet(‘/content/prices.parquet')

<img width="841" alt="Screen Shot 2022-09-13 at 10 07 02" src="https://user-images.githubusercontent.com/5858494/189798714-953b2f3e-31a3-4ee1-974b-2b00d97efd8d.png">

df_parquet = pd.read_parquet('/content/prices.parquet')
df_parquet.head()


<img width="848" alt="Screen Shot 2022-09-13 at 10 07 20" src="https://user-images.githubusercontent.com/5858494/189798746-05159d9b-4164-437a-9403-a686df566618.png">

<img width="858" alt="Screen Shot 2022-09-13 at 10 07 36" src="https://user-images.githubusercontent.com/5858494/189798783-c363b4b4-e2bc-4f75-a07b-c08b9ab79776.png">

References:
Levkovsky M,. (2019, Jun 13). CSV vs Parquet vs Avro: Choosing the Right Tool for the Right Job. Medium. https://medium.com/ssense-tech/csv-vs-parquet-vs-avro-choosing-the-right-tool-for-the-right-job-79c9f56914a8
Spicer T,. (2019, May 28). Apache Parquet vs. CSV Files. DZone. https://dzone.com/articles/how-to-be-a-hero-with-powerful-parquet-google-and
