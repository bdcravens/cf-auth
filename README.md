cf-auth
=======

Authentication framework for ColdFusion/CFML similar to Devise + OmniAuth

Goals:

* Build on my talks at cf.Objective() 2012 and NCDevCon 2012 - Rather than doing federated identity as a series of disconnected components, let's have a unified framework
* Basic framework that can be extended via a number of strategies, like Devise + Omniauth
* Support popular login mechanisms: session+database, session+ORM, Twitter, Facebook, Google, other oAuth/oAuth2/OpenID identity providers
* Add features commonly seen and reimplemented: hashed passwords, remember session, forgot password, confirmation, validation, invitation
* ColdFusion has a login framework: CFLogin and associated tags. Problem is, it falls short. However, we don't have to throw out the baby with the bath wataer. Can we build atop the framework already in place?
* Must be extendable. Provide reasonable defaults, while giving user ability to override anything.
* Framework agnostic, but easily integrated into any framework.
* ColdFusion compatibility: ACF 8, 9, 10  / Railo 3 + / OpenBlueDragon 2.0+