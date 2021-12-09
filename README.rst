oxipng pre-commit mirror
========================

Mirror of `oxipng <https://github.com/shssoichiro/oxipng>`__ for `pre-commit <https://pre-commit.com>`__.

Installation
------------

Add to your pre-commit config:

.. code-block:: yaml

    -   repo: https://github.com/adamchainz/pre-commit-oxipng
        rev: ''  # Use the sha / tag you want to point at
        hooks:
        -   id: oxipng

By default all PNG files are passed to oxipng with the default settings, which provides reasonable optimization.
