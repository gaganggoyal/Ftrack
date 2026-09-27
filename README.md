# Ftrack

A stock portfolio tracker in Rails. Users sign up, look up a ticker, add it to
their portfolio, and follow friends to see what they are holding.

- Sign-up and login with Devise (with Bootstrap-styled views)
- Live quotes from the IEX Cloud API through `iex-ruby-client`
- A many-to-many `user_stocks` join for portfolios and a self-referential
  `friendships` table for following other users
- A search to find friends by name or email

**Stack:** Ruby 2.7, Rails 6.1, SQLite in development, PostgreSQL in production

## Run it

```bash
bundle install
bin/rails db:setup
bin/rails server
```

Set your IEX API keys in Rails credentials before looking up stocks.

---

An early learning project from 2023, kept for reference and archived. My current work is on [my profile](https://github.com/gaganggoyal) and at [gagan.indiaoffers.in](https://gagan.indiaoffers.in).
