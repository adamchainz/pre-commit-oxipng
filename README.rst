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

Optimizing all the PNG’s in your repository is expensive and won’t produce results often.
You probably want to skip oxipng on your CI system, and run it only on commit.
On `pre-commit.ci <https://pre-commit.ci/#configuration>`__ declare it to be skipped like so:

.. code-block:: yaml

    ci:
      skip:
      - oxipng

On other CI systems, use pre-commit’s ``SKIP`` environment variable.
