![Base Branch](https://img.shields.io/badge/base%20branch-trunk-important)
![GitHub License](https://img.shields.io/github/license/andrewmcodes/sheepdog)
![OSS Lifecycle](https://img.shields.io/osslifecycle/andrewmcodes/sheepdog)
![Last Commit To Trunk](https://img.shields.io/github/last-commit/andrewmcodes/sheepdog/trunk)
![Last Commit](https://img.shields.io/github/last-commit/andrewmcodes/sheepdog)

# Prometheus + Grafana Demo Rails App

Ruby on Rails application initialized with all the good stuff. Use at your own risk or we welcome pull requests. I will be working on a roadmap soon.

## Setup

Please take note that we are using `trunk` as the base branch.

![Base Branch](https://img.shields.io/badge/base%20branch-trunk-important)

### System dependencies

- Ruby version: 2.7.1
- Rails version: 6.0.3.1
- Database: PostgreSQL
- Redis installed

### Configuration

Copy an existing sample environment file. Run:
```bash
$ cp .env.sample .env
```

and edit newly created `.env` file. The minimum you are going to need are
credentials to your local PostgreSQL database.

Then, install all the necessary gems:
```bash
bundle install
```

### Database creation

In order to create the database with all the necessary seed data, run:
```bash
$ rails db:create db:schema:load db:seed
```

### How to start the app

Start the Ruby on Rails server with:
```bash
rails server
```
To run Sidekiq, launch another process with:
```bash
bundle exec sidekiq
```

### Code quality checks

The application provides the following code quality analysis tools:

- [Brakeman][brakeman]
- [Fasterer][fasterer]
- [Rails Best Practices][rails-best-practices]
- [Bundler Audit][bundler-audit]

To run them locally:

```bash
$ bundle exec brakeman
$ bundle exec fasterer
$ bundle exec rails_best_practices
$ bundle audit
```

[brakeman]: https://github.com/presidentbeef/brakeman
[fasterer]: https://github.com/DamirSvrtan/fasterer
[rails-best-practices]: https://github.com/flyerhzm/rails_best_practices
[bundler-audit]: https://github.com/rubysec/bundler-audit

### Changelog

Coming Soon
<!-- [View our Changelog][changelog] -->

### Contributing

Coming Soon
<!-- [Contributing Guide][contributing] -->

### Code of Conduct

[Code of Conduct][coc]

### License

[MIT][license]


[changelog]: /CHANGELOG.md
[coc]: /CODE_OF_CONDUCT.md
[contributing]: /CONTRIBUTING.md
[license]: /LICENSE
