<!---
    This file is part of pymice-tools.
    Copyright (C) 2018-2019  Emir Turkes

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

    Emir Turkes can be contacted at eturkes@bu.edu
-->

# PyMICE Tools
#### *This project is currently under unstable development*

PyMICE Tools is companion to the PyMICE library for Intellicage analysis
(https://github.com/Neuroinflab/PyMICE). The two are not directly affiliated. The goal
of PyMICE Tools is to extend the functionality and usuability of PyMICE by providing
user interfaces, a standardized method for adding high-level experimental and
statistical routines, and project templates that foster reproducible research.

This is a meta repository to consolidate installation of three distinct submodules:
* PyMICE Modules (https://github.com/eturkes/pymice-modules)
* PyMICE Analyzer (https://github.com/eturkes/pymice-analyzer)
* PyMICE Server (https://github.com/eturkes/pymice-server)

PyMICE Modules is dedicated to the development of PyMICE *paradigms*, high-level
routines as simple as calculating corner visits to analyzing following behaviors.
Addition of statistical and figure generation methods, as well as miscellaneous
utilities also go here. The goal is to establish a standardized API for working with the
upstream PyMICE library. This has the potential of making the analysis pipeline highly
modular, which will offer the user great flexibility in creating custom pipelines and
implementing tools and techniques from third-party projects.

PyMICE Analyzer is a GUI and CLI project creator and pipeline manipulator. It is
distinct from full-featured platforms in that it leverages the power and familiarity of
standard data science tools like Jupyter and Docker. Projects are structured to suit the
particular workflow of Intellicage with PyMICE and are bundled with a variety of
utilities to encourage proper archivial for reproducibility. Available pipeline options
are pulled directly from PyMICE Modules and included in the project structure, allowing
for easy updating and shipping of specific versions with the code.

PyMICE Server has a similar workflow and functionality to PyMICE Analyzer but utilizes
Wooey (https://github.com/wooey/Wooey) to create a Django-based web UI. A noteworthy
advantage is that it is easily configured so that jobs are submitted to local or cloud
servers for centralized, high-throughput analysis. For laboratories interesting in
applying techniques with high hardware demands like machine learning, this may be a
useful tool.
