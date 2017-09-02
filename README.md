## History

```
python ../python/spark-warehouse/generate_budget.py budget.json

python -m json.tool ads.txt

python ../../python/spark-warehouse/dedupe_ads.py ../crawled/ads.txt clean_ads1.txt

python generate_user.py user_small.txt

python ../python/spark-warehouse/generate_query_ad.py ../data/deduped/clean_ads.txt query_camp_ad_file.json campaign_weight_file.json ad_weight_file.json query_group_id_query_file.json campaignId_category_file.json campaignId_adId_file.json

python ../python/spark-warehouse/generate_click_log.py ../data/deduped/clean_ads.txt ../data/log/user_small.txt query_camp_ad_file.json campaign_weight_file.json ad_weight_file.json campaignId_category_file.json campaignId_adId_file.json click_log_small.txt

install j2ee eclipse
install mysql

install mysql-connector for java

install mysql-workbench

```

```sql
CREATE TABLE `ad` (
`adId` int(11) NOT NULL,
`campaignId` int(11) DEFAULT NULL,
`keyWords` varchar(1024) DEFAULT NULL,
`bidPrice` double DEFAULT NULL,
`price` double DEFAULT NULL,
`thumbnail` mediumtext,
`description` mediumtext,
`brand` varchar(100) DEFAULT NULL,
`detail_url` mediumtext,
`category` varchar(1024) DEFAULT NULL,
`title` varchar(2048) DEFAULT NULL,
PRIMARY KEY (`adId`)
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```

```sql
CREATE TABLE `campaign` (
`campaignId` int(11) NOT NULL,
`budget` double DEFAULT NULL,
PRIMARY KEY (`campaignId`)
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
