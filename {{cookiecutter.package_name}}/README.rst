{{ cookiecutter.package_name.split('.') | map('capitalize') | join(' ') }}
{{ "=" * cookiecutter.package_name.__len__() }}

{{ cookiecutter.description }}

Run the Tests
-------------
    
Install tox and run it::

    pip install tox
    tox

Limit the tests to a specific python version::

    tox -e py27

Conventions
-----------

{{ cookiecutter.package_name.split('.') | map('capitalize') | join(' ') }} follows PEP8 as close as possible. To test for it run::

    tox -e pep8

{{ cookiecutter.package_name.split('.') | map('capitalize') | join(' ') }} uses `Semantic Versioning <http://semver.org/>`_

Build Status
------------

.. image:: https://travis-ci.org/OneGov/{{ cookiecutter.package_name }}.png
  :target: https://travis-ci.org/OneGov/{{ cookiecutter.package_name }}
  :alt: Build Status

Coverage
--------

.. image:: https://coveralls.io/repos/OneGov/{{ cookiecutter.package_name }}/badge.png?branch=master
  :target: https://coveralls.io/r/OneGov/{{ cookiecutter.package_name }}?branch=master
  :alt: Project Coverage

Latests PyPI Release
--------------------
.. image:: https://pypip.in/v/{{ cookiecutter.package_name }}/badge.png
  :target: https://crate.io/packages/{{ cookiecutter.package_name }}
  :alt: Latest PyPI Release

License
-------
{{ cookiecutter.package_name }} is released under GPLv2
