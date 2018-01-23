# Rail with Ruby
FROM ruby
COPY sources.list /etc/apt/

RUN apt-get update \
  && apt-get install -y build-essential libpq-dev \
  && apt-get clean all \
  && rm -rf /var/lib/apt/lists/* \
  && mkdir /mydir
WORKDIR /mydir
COPY Gemfile /mydir/Gemfile
RUN bundle install
COPY . /mydir
