.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
    :alt: License: AGPL-3

==========================================================
Customizable unsubscription process on mass mailing emails
==========================================================

With this module you can set a custom unsubscribe link appended at the bottom
of mass mailing emails.


Configuration
=============

To configure unsubscribe label go to *Settings > Technical > Parameters >
System parameters* and add a ``mass_mailing.unsubscribe.label`` parameter
with HTML to set at the bottom of mass emailing emails. Including ``%(url)s``
variable where unsubscribe link.

For example::

    <small>You can unsubscribe <a href="%(url)s">here</a></small>

Additionally, you can disable this link if you set this parameter to ``False``.

If this parameter (``mass_mailing.unsubscribe.label``) does not exist, the
default 'Click to unsubscribe' link will appear, with the advantage that it is
translatable via *Settings > Translations > Application Terms > Translated
terms*.

Also your unsubscriptors will recieve a beautier goodbye page. You can
customize it clicking here **after installing the module**:

* `Unsubscription successful </page/mass_mail_unsubscription_success>`_.
* `Unsubscription failed </page/mass_mail_unsubscription_failure>`_.


Usage
=====

.. image:: https://odoo-community.org/website/image/ir.attachment/5784_f2813bd/datas
   :alt: Try me on Runbot
   :target: https://runbot.odoo-community.org/runbot/205/8.0


Known issues / Roadmap
======================

* This custom HTML is not translatable, so as a suggestion, you can define
  the same text in several languages in several lines.

For example:

.. code:: html

  <small>[EN] You can unsubscribe <a href="%(url)s">here</a></small><br/>
  <small>[ES] Puedes darte de baja <a href="%(url)s">aquí</a></small>


Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/social/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback
`here <https://github.com/OCA/social/issues/new?body=module:%20mass_mailing_custom_unsubscribe%0Aversion:%208.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.


Credits
=======

Contributors
------------

* Rafael Blasco <rafabn@antiun.com>
* Antonio Espinosa <antonioea@antiun.com>
* Jairo Llopis <yajo.sk8@gmail.com>

Maintainer
----------

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.
