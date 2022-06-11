# Django-ElasticSearch



# Download and install archive for Linux
wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.2.2-linux-x86_64.tar.gz
wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.2.2-linux-x86_64.tar.gz.sha512
shasum -a 512 -c elasticsearch-8.2.2-linux-x86_64.tar.gz.sha512 
tar -xzf elasticsearch-8.2.2-linux-x86_64.tar.gz
cd elasticsearch-8.2.2/ 

# Download and install archive for MacOSedit
curl -O https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.2.2-darwin-x86_64.tar.gz
curl https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.2.2-darwin-x86_64.tar.gz.sha512 | shasum -a 512 -c - 
tar -xzf elasticsearch-8.2.2-darwin-x86_64.tar.gz
cd elasticsearch-8.2.2/ 

# if you face any error please go through this link
https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html#install-macos

# After installation run this command in your terminal
$ docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.14.0

# Final EndPoinnts
http://127.0.0.1:8000/search/user/mike/	Returns user 'mike13'

http://127.0.0.1:8000/search/user/jess_/	Returns user 'jess_'

http://127.0.0.1:8000/search/category/seo/	Returns category 'SEO optimization'

http://127.0.0.1:8000/search/category/progreming/	Returns category 'Programming'

http://127.0.0.1:8000/search/article/linux/	Returns article 'Installing the latest version of Ubuntu'

http://127.0.0.1:8000/search/article/java/	Returns article 'Which programming language is the best?'

