# Rail with Ruby
FROM ruby
COPY sources.list /etc/apt/

RUN apt-get update \
  && apt-get install build-essential libpq-dev \
  && apt-get clean all \
  && rm -rf /var/lib/apt/lists/* \
  && mkdir /mydir
WORKDIR /mydir
COPY Gemfile /mydir
RUN bundle install
ADD . /mydir
