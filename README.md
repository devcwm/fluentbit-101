## Commands

# Standard output

fluent-bit -c configs/apache_common.yml

# Apache parsing stdout

fluent-bit -c configs/apache_common.yml -R parsers/parsers.conf

# Java multiline stdout

fluent-bit -c configs/multiline_nested.yml

# Java multiline parsing stdout 

fluent-bit -c configs/multiline_nested.yml -R parsers/parsers_multiline.conf

# Spring app stdout

fluent-bit -c configs/spring_app.yml

# Spring app regex parser stdout

fluent-bit -c configs/spring_app.yml -R parsers/parsers_spring.conf

# Spring app filter info

fluent-bit -c configs/spring_app_filter.yml -R parsers/parsers_spring.conf

# Spring app json output

fluent-bit -c configs/spring_app_filter.yml -R parsers/parsers_spring.conf | jq 