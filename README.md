## History

```
python ../python/spark-warehouse/generate_budget.py budget.json

python -m json.tool ads.txt

python ../../python/spark-warehouse/dedupe_ads.py ../crawled/ads.txt clean_ads1.txt

python generate_user.py user_small.txt

python ../python/spark-warehouse/generate_query_ad.py ../data/deduped/clean_ads.txt query_camp_ad_file.json campaign_weight_file.json ad_weight_file.json query_group_id_query_file.json campaignId_category_file.json campaignId_adId_file.json

python ../python/spark-warehouse/generate_click_log.py ../data/deduped/clean_ads.txt ../data/log/user_small.txt query_camp_ad_file.json campaign_weight_file.json ad_weight_file.json campaignId_category_file.json campaignId_adId_file.json click_log_small.txt
```
