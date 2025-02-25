# OpenID Connect / OAuth client

The OpenID Connect module provides a pluggable client implementation for the
OpenID Connect protocol. The server implementation of the protocol is provided
by OAuth2 Server.

OpenID Connect 1.0 is a simple identity layer on top of the OAuth 2.0 protocol.
It allows Clients to verify the identity of the End-User based on the
authentication performed by an Authorization Server, as well as to obtain basic
profile information about the End-User in an interoperable and REST-like manner.

For a full description of the module, visit the
[project page](https://www.drupal.org/project/openid_connect).

Submit bug reports and feature suggestions, or track changes in the
[issue queue](https://www.drupal.org/project/issues/openid_connect).


## Contents of this file

- Usage
- Requirements
- Features
- Installation
- Configuration
- Troubleshooting


## Usage

The module allows you to use an external OpenID Connect login provider to
authenticate and log in users on your site. If a user signs in with a login
provider for the first time on the website, a new Drupal user will be created.
Google for instance uses OpenID Connect to authenticate users across all of
their services.


## Requirements

This module requires no modules outside of Drupal core.


## Features

- Supported login providers
- Login with Google
- Client configuration
- Fetching user profile information
- Sign in block

For a more detailed description and instructions please refer to the
documentation [client configuration](https://www.drupal.org/node/2274339).

**Permissions:**

The module adds a new permission section entitled OpenID Connect API with
three new user rights:

- Administer OpenID Connect clients
- Manage own connected accounts
- Set a password for local authentication.


## Installation

Install as you would normally install a contributed Drupal module.
Visit [project page](https://www.drupal.org/project/openid_connect) and
[Installing Drupal Modules](https://www.drupal.org/docs/extending-drupal/installing-drupal-modules)
for further information.


## Configuration

Configuration options are available at

`Administration >> Configuration >> Services >> OpenID Connect`

You can enable clients for login providers and configure their client ID and
client secret which are necessary credentials for authenticating with an OAuth2
server.


## Troubleshooting

A standard Drupal block is available to sign in with the login providers for
which clients are enabled.
A single button is shown for each login provider.
In case if the login block does not display on the user's login page, check it
in the blocks list `Administration >> Structure >> Block layout`
