|TASKS|DESCRIPTION|
| :-- | :-- |
| rake about                                                             | # List versions of all Rails frameworks and the environment
| rake add_topic_to_quotes                                               | # Add the topic to quotes
| rake admin:create                                                      | # Creates a forum administrator
| rake admin:invite[email]                                               | # invite an admin to this discourse instance
| rake annotate                                                          | # ensure the asynchronously-created post_search_data index is present
| rake annotate:clean                                                    | # regenerate core model annotations using a temporary database
| rake annotate:ensure_all_indexes                                       | # ensure the asynchronously-created post_search_data index is present
| rake api_key:create_master[description]                                | # generate a master api key with given description
| rake app:template                                                      | # Applies the template supplied by LOCATION=(/path/to/template) or URL
| rake app:update                                                        | # Update configs and some other initially generated files (or use just update:configs or update:bin)
| rake assets:clean[keep]                                                | # Remove old compiled assets
| rake assets:clobber                                                    | # Remove compiled assets
| rake assets:environment                                                |# Load asset compile environment
| rake assets:precompile                                                 |# Compile all the assets named in config.assets.precompile
| rake assets:prestage                                                   |# pre-stage assets on cdn
| rake autospec                                                          |# Run all specs automatically as needed
| rake autospec:swagger                                                  |# Regenerate swagger docs on API spec change
| rake avatars:clean                                                     |# Clean up all avatar thumbnails (use this when the thumbnail algorithm changes)
| rake avatars:refresh                                                   |# Refresh all avatars (download missing gravatars, refresh system)
| rake cache_digests:dependencies                                        |# Lookup first-level dependencies for TEMPLATE (like messages/show or comments/_comment.html)
| rake cache_digests:nested_dependencies                                 |# Lookup nested dependencies for TEMPLATE (like messages/show or comments/_comment.html)
| rake categories:list                                                   |# Output a list of categories
| rake categories:populate                                               |# Creates sample categories
| rake db:create                                                         |# Creates the database from DATABASE_URL or config/database.yml for the current RAILS_ENV (use db:create:all to create all databases in the config). Without RAIL...
| rake db:drop                                                           |# Drops the database from DATABASE_URL or config/database.yml for the current RAILS_ENV (use db:drop:all to drop all databases in the config). Without RAILS_ENV ...
| rake db:environment:set                                                |# Set the environment value for the database
| rake db:fixtures:load                                                  |# Loads fixtures into the current environment's database
| rake db:migrate:down                                                   |# Runs the "down" for a given migration VERSION
| rake db:migrate:redo                                                   |# Rolls back the database one migration and re-migrates up (options: STEP=x, VERSION=x)
| rake db:migrate:status                                                 |# Display status of migrations
| rake db:migrate:up                                                     |# Runs the "up" for a given migration VERSION
| rake db:prepare                                                        |# Runs setup if database does not exist, or runs migrations if it does
| rake db:rebuild_indexes                                                |# Rebuild indexes
| rake db:reset                                                          |# Drops and recreates the database from db/schema.rb for the current environment and loads the seeds
| rake db:schema:cache:clear                                             |# Clears a db/schema_cache.yml file
| rake db:schema:cache:dump                                              |# Creates a db/schema_cache.yml file
| rake db:schema:dump                                                    |# Creates a database schema file (either db/schema.rb or db/structure.sql, depending on `config.active_record.schema_format`)
| rake db:schema:load                                                    |# Loads a database schema file (either db/schema.rb or db/structure.sql, depending on `config.active_record.schema_format`) into the database
| rake db:seed                                                           |# Loads the seed data from db/seeds.rb
| rake db:seed:replant                                                   |# Truncates tables of each database for current environment and loads the seeds
| rake db:seed_fu                                                        |# Loads seed data for the current environment
| rake db:setup                                                          |# Creates the database, loads the schema, and initializes with the seed data (use db:reset to also drop the database first)
| rake db:stats                                                          |# Statistics about database
| rake db:status:json                                                    |# Check that the DB can be accessed
| rake db:structure:dump                                                 |# Dumps the database structure to db/structure.sql
| rake db:structure:load                                                 |# Recreates the databases from the structure.sql file
| rake db:validate_indexes[arg]                                          |# Validate indexes
| rake db:version                                                        |# Retrieves the current schema version number
| rake destroy:categories                                                |# Destroy a comma separated list of category ids
| rake destroy:groups                                                    |# Destroy all groups
| rake destroy:private_messages                                          |# Remove all private messages
| rake destroy:stats                                                     |# Destroy site stats
| rake destroy:topics[category,parent_category]                          |# Remove all topics in a category
| rake destroy:topics_all_categories                                     |# Remove all topics in all categories
| rake destroy:users                                                     |# Destroy all non-admin users
| rake dev:config                                                        |# Initialize development environment
| rake dev:populate                                                      |# Populate sample content for development environment
| rake dev:repopulate                                                    |# Repopulate sample datas in development environment
| rake dev:reset                                                         |# Run db:migrate:reset task and populate sample content for development environment
| rake discourse_checklist:migrate_old_syntax                            |# Convert old style checkbox markdown to new style
| rake docker:test                                                       |# Run all tests (JS and code in a standalone environment)
| rake emails:import                                                     |# use this task to import a mailbox into Discourse
| rake emails:test[email]                                                |# Check if SMTP connection is successful and send test message
| rake emoji:test                                                        |# test the emoji generation script
| rake emoji:update                                                      |# update emoji images
| rake enqueue_digest_emails                                             |# This task is called by the Heroku scheduler add-on
| rake export:categories[category_ids]                                   |# Export all the categories
| rake export:category_structure[include_group_users,file_name]          |# Export only the structure of all categories
| rake export:groups[include_group_users,file_name]                      |# Export all user groups
| rake follow:install:migrations                                         |# Copy migrations from follow to application
| rake groups:populate                                                   |# Creates sample categories
| rake i18n:check                                                        |# Checks locale files for errors
| rake i18n:reseed[locale]                                               |# Update seeded topics and categories with latest translations
| rake import:file[file_name]                                            |# Import existing exported file
| rake import:update_first_post_created_at                               |# Update first_post_created_at column in user_stats table
| rake incoming_emails:truncate_long                                     |# removes attachments and truncates long raw message
| rake integration:create_fixtures                                       |# Creates the integration fixtures
| rake log:clear                                                         |# Truncates all/specified *.log files in log/ to zero bytes (specify which logs with LOGS=test,development)
| rake maxminddb:get                                                     |# downloads MaxMind's GeoLite2-City database
| rake middleware                                                        |# Prints out your Rack middleware stack
| rake multisite:generate:config                                         |# generate multisite config file (if missing)
| rake multisite:rollback                                                |# rollback migrations for all sites in tier
| rake plugin:install[repo]                                              |# install plugin
| rake plugin:install_all_gems                                           |# install all plugin gems
| rake plugin:install_all_official                                       |# install all official plugins (use GIT_WRITE=1 to pull with write access)
| rake plugin:install_gems[plugin]                                       |# install plugin gems
| rake plugin:migrate:down[plugin]                                       |# run all migrations of a plugin
| rake plugin:pull_compatible[plugin]                                    |# pull a compatible plugin version
| rake plugin:pull_compatible_all                                        |# pull compatible plugin versions for all plugins
| rake plugin:qunit[plugin,timeout]                                      |# run plugin qunit tests
| rake plugin:spec[plugin]                                               |# run plugin specs
| rake plugin:update[plugin]                                             |# update a plugin
| rake plugin:update_all                                                 |# update all plugins
| rake plugin:versions                                                   |# display all plugin versions
| rake poll:migrate_old_polls                                            |# Migrate old polls to new syntax
| rake post_revisions:populate                                           |# Create post revisions
| rake posts:delete_all_likes                                            |# Delete all likes
| rake posts:delete_word[find,type,ignore_case]                          |# Delete occurrence of a word/string
| rake posts:fix_letter_avatars                                          |# Rebake all posts with a quote using a letter_avatar
| rake posts:inline_uploads                                              |# Coverts full upload URLs in `Post#raw` to short upload url
| rake posts:invalidate_broken_images                                    |# invalidate broken images
| rake posts:missing_uploads                                             |# Finds missing post upload records from cooked HTML content
| rake posts:normalize_code                                              |# normalize all markdown so <pre><code> is not used and instead backticks
| rake posts:rebake                                                      |# Update each post with latest markdown
| rake posts:rebake_match[pattern,type,delay]                            |# Rebake all posts matching string/regex and optionally delay the loop
| rake posts:recover_uploads_from_index                                  |# Attempts to recover missing uploads from an index file
| rake posts:refresh_emails[topic_id]                                    |# Refreshes each post that was received via email
| rake posts:refresh_oneboxes                                            |# Update each post with latest markdown and refresh oneboxes
| rake posts:remap[find,replace,type,ignore_case]                        |# Remap all posts matching specific string
| rake posts:reorder_posts[topic_id]                                     |# Reorders all posts based on their creation_date
| rake qunit:test[timeout,qunit_path]                                    |# Runs the qunit test suite
| rake reactions:generate[post_id,reactions_count,reaction]              |# create users and generate random reactions on a post
| rake release_note:generate[from,to,repo]                               |# generate a release note from the important commits
| rake release_note:plugins:generate[from,to,plugin_glob,org]            |# generate release notes for all official plugins in a directory
| rake replies:populate[topic_id,count]                                  |# Add replies to a topic
| rake restart                                                           |# Restart app by touching tmp/restart.txt
| rake scheduler:run_all                                                 |# run every task the scheduler knows about in that order, use only for debugging
| rake secret                                                            |# Generate a cryptographically secure secret key (this is typically used to generate a secret for cookie sessions)
| rake site:export_structure[zip_path]                                   |# Exports site structure (settings, groups, categories, tags, themes, etc) to a ZIP file
| rake site:import_structure[zip_path]                                   |# Imports site structure from a ZIP file exported by site:export_structure
| rake site_settings:export                                              |# Exports site settings
| rake site_settings:import                                              |# Imports site settings
| rake smoke:test                                                        |# run chrome headless smoke tests on current build
| rake stats                                                             |# Report code statistics (KLOCs, etc) from the application or engine
| rake tags:populate                                                     |# Creates sample tags
| rake themes:audit                                                      |# List all the installed themes on the site
| rake themes:install                                                    |# Install themes & theme components
| rake themes:isolated_test                                              |# Install a theme/component on a temporary DB and run QUnit tests
| rake themes:qunit[type,value]                                          |# Run QUnit tests of a theme/component
| rake themes:update                                                     |# Update themes & theme components
| rake time:zones[country_or_offset]                                     |# List all time zones, list by two-letter country code (`bin/rails time:zones[US]`), or list by UTC offset (`bin/rails time:zones[-8]`)
| rake tmp:clear                                                         |# Clear cache, socket and screenshot files from tmp/ (narrow w/ tmp:cache:clear, tmp:sockets:clear, tmp:screenshots:clear)
| rake tmp:create                                                        |# Creates tmp directories for cache, sockets, and pids
| rake topics:populate                                                   |# Creates sample topics
| rake users:anonymize_all                                               |# Anonymize all users except staff
| rake users:change_post_ownership[old_username,new_username,archetype]  |# Change topic/post ownership of all the topics/posts by a specific user (without creating new revision)
| rake users:disable_2fa[username]                                       |# Disable 2FA for user with the given username
| rake users:list_recent_staff                                           |# List all users which have been staff in the last month
| rake users:merge[source_username,target_username]                      |# Merge the source user into the target user
| rake users:populate                                                    |# Creates sample user accounts
| rake users:recalculate_post_counts                                     |# Recalculate post and topic counts in user stats
| rake users:rename[old_username,new_username]                           |# Rename a user
| rake users:update_posts[old_username,current_username]                 |# Update username in quotes and mentions
| rake yarn:install                                                      |# Install all JavaScript dependencies as specified via Yarn
| rake zeitwerk:check                                                    |# Checks project structure for Zeitwerk compatibility
