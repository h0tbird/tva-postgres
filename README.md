<img src="http://45.media.tumblr.com/0370959cd51e9ffd354f8f2e825c05c3/tumblr_n6jwtyRzcU1rwdgsoo1_1280.gif"
  align="right" border="0" width="128" height="128" />

# docker-tva-postgres

[![Build Status](https://travis-ci.org/katosys/docker-tva-postgres.svg?branch=master)](https://travis-ci.org/katosys/docker-tva-postgres)

Containerized PostgreSQL service.

#### clone

Do not clone this repository.  
The control repository is named `the-voting-app`.  
Perform a recursive clone of the control repository:

```
git clone --recursive ${GIT_SERVER_URL}/the-voting-app.git
```

#### Tip

Run the command below to query the `votes` table:

```
docker exec -it <docker-id> /bin/bash -c "psql -U postgres -d postgres -c 'SELECT * FROM votes'"
```
