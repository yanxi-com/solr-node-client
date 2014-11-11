[![NPM](https://nodei.co/npm/solr-client.png?downloads=true&stars=true)](https://nodei.co/npm/solr-client2/)

Please see https://github.com/lbdremy/solr-node-client

Seems above didn't have highlight support, Only add Query.customer(key, value)

For example, you can use query below to highlight title:

```
  query = solrClient.createQuery().q
    title: 'xxx' 
  .customer 'hl', 'true'
  .customer 'hl.fl', 'title'
```
