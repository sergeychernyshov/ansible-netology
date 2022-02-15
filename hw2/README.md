#1 что делает playbook 

    Плейбук скачивает архивы с инсталляторами на целевые хосты.
    На все хосты загружаем архив с JAVA.
    На хост elasticsearch загружаем архив elasticsearch.
    На хост kibana архив с kibana.
    
    Производим распаковку архивов во временные директории.


#2 какие у него есть параметры и теги

    Параметры
        java_jdk_version
        java_home
        elastic_version
        elastic_home
        kibana_version
        kibana_home
    
    Теги
        java
        elastic
        kibana

    
    