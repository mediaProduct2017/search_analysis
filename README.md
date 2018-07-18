# search_analysis

[elastic_search](https://github.com/arfu2016/nlp/tree/master/nlp_models/elasticSearch)

运行elasticsearch

下载地址：
https://www.elastic.co/downloads/elasticsearch 

cd ~/setups/elasticsearch-6.2.4/bin 

$./elasticsearch

把问句和实体标签存入es，并对问句或实体标签做查询

[ask2](https://github.com/arfu2016/nlp/tree/master/nlp_models/elasticSearch/ask2)

elastic search可用于模糊查询，一种是句子的模糊查询，用match来做（精确查询是用term），这种模糊查询是基于句子中的词的，看句子中词的匹配程度（所以怎样分词也具有很大的影响），看重叠程度有多大，不是基于句向量的。另一种是词的模糊查询，也就是[fuzzy query](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-fuzzy-query.html)，在这种查询下，词不一定要完全匹配，fuziness设定了编辑距离，在设定的编辑距离以内都算匹配。
