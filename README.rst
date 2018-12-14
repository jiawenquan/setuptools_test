===================================
setuptools_test |Build Status|
===================================
   :target: https://github.com/jiawenquan/setuptools_test


这是一个 `setuptools <https://github.com/pypa/setuptools>`_ 的使用案例

This is a `setuptools <https://github.com/pypa/setuptools>`_  use case


Prerequisites
##############

- python 3.6 or 3.*
- windows10 or linux
- pip >= 18.1

Installing
#############
    .. code-block:: bash

        conda create -n setuptools_env python=3.6
        activate setuptools_env
        (setuptools_env) pip install -U setuptools
        (setuptools_env) git clone https://github.com/jiawenquan/setuptools_test
        (setuptools_env) cd setuptools_test
        (setuptools_env) ..\setuptools_test> pip install -e .
        (setuptools_env) ..\setuptools_test> python setup.py install


Running the tests
###################
    .. code-block:: bash

        $ activate setuptools_env
        (setuptools_env) $ setuptools_test
        我希望有个如你一般的人


Usage
######
- Generate the package file
    .. code-block:: bash

        python setup.py bdist_egg      # *.egg files are generated and easy_install is supported

        python setup.py bdist_wininst  # Generate the *.exe file

        python setup.py sdist          # Generate *.zip/*.tar.gz files to support pip installation

        python setup.py bdist_wheel    # Generate.whl files

- Installation of packaging files
    .. code-block:: bash

        python setup.py install  # The source code installation

        easy_install *.egg     # .egg file installation

        easy_install *.zip/*.tar.gz     # .zip file installation

        pip install *.whl      # .whl file installation




Authors
##########
* **jiawenquan** - *Initial work* - [jiawenquan](https://github.com/jiawenquan)

Versioning
############
`Version: 1.0.1`

Licence
##########

Copyright © 2018 jiawenquan (@Tofull) and contributors
Distributed under the MIT Licence.
