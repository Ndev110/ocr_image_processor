# OCR App
Welcome to Image OCR App! This is a one-page version of a Image OCR App. The app allows user to upload a png image and extract text data from it. It also allows the user to search on the document provided and process by the OCR App.
## Getting Started
To get started with the OCR App, please follow the instructions below:
1. git clone ''
2. Navigate to the project directory using your command prompt or terminal.
3. Run the command bundle install to install all necessary dependencies.
## Tech Stack
The tech stack used to build OCR App are:
* Ruby on Rails - a web application framework written in the Ruby programming language
* PostgreSQL - an open-source relational database management system
## Dependencies
The following dependencies are required to run OCR App:
* Ruby 3.0.2
* Rails 7.1.3
* PostgreSQL 15
* Redis
* ImageMagick
* rtesseract
## Installation Guide
>#### Install [RVM](https://rvm.io/rvm/install)
Install the right ruby version (currently 3.0.2):
```shell
  rvm install "ruby-3.0.2"
```
>#### Check your Ruby version
```shell
  ruby -v
```
The ouput should start with something like `ruby 3.0.2`
>#### Install Database (PostgreSQL) 15
```shell
  brew install postgresql
  brew services start postgresql
```
>#### Install Redis
```shell
  brew install redis
  brew services start redis
```
#### Install ImageMagick
```shell
  brew install imagemagick
```
#### Install rtesseract
[Documentation](https://github.com/dannnylo/rtesseract)
```shell
  brew install tesseract
```
### Run this command to install all gems and dependencies
```
bundle install or bundle
```
## Database Setup:
```sh
rails db:create
rails db:migrate
```
## Linting
[Rubocop](https://github.com/bbatsov/rubocop) linter is configured for this project. In order to trigger linting via CLI, run in root project's folder:
```
rubocop
```
However if you use Rails scaffolding features, autogenerated code may fail under some of the Rubocop's configured rules. Luckily *Rubocop* supports auto-correction, so you can fix auto-generated code running:
```
rubocop -A
```
## Running up the Server
```sh
bundle exec rails s
```
Once the server is running, you can access the application by navigating to http://localhost:3000 in your web browser.
## Functionality
With OCR APP, you can perform the following actions:
1. Upload an png image

3. Get the marked bounded box image with the extracted text highlighted
3. Search text on image
4. User can download the original and modified image

## Feedback
If you have any feedback or suggestions for improving OCR APP, please feel free to reach out to me. I would love to hear from you!