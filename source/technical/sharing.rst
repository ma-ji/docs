.. _trovi:

====================
Trovi sharing portal
====================

`Chameleon Trovi <https://www.chameleoncloud.org/experiment/share>`_ is a
sharing portal that allows you to share digital research and education
artifacts, such as packaged experiments, workshop tutorials, or class materials.
Each research artifact is represented as a deposition (a remotely accessible
folder) where a user can put Jupyter notebooks, links to images, orchestration
templates, data, software, and other digital representations that together
represent a focused contribution that can be run on Chameleon. Users can use
these artifacts to recreate and rerun experiments or class exercises on a
Jupyter Notebook within Chameleon. They can also create their own artifacts and
publish them directly to Trovi from within :ref:`Chameleon's Jupyter server
<jupyter>`.

To get started, find the "Trovi" dropdown option under the "Experiment" section
of chameleoncloud.org. Once you're on the Trovi homepage, you'll see a list of
publicly available experiments and other digital artifacts. You can now browse
those artifacts or upload your own.

.. figure:: sharing/sharing_dropdown.png
   :alt: Location of Trovi in the UI.
   :figclass: screenshot

   The "Trovi" option under the "Experiment" section takes you to Trovi.

Browsing artifacts
==================

Trovi allows you to browse artifacts, presented in a scrolling list format. On
the right hand side, there are multiple filtering options. By clicking on the
project name, you can see all the artifacts that belong to that project. The
"All" choice shows you all of the artifacts you have access to. You can also see
how many times people have downloaded and launched your notebook with the icons
in the bottom left corner of an artifact.

Launching an artifact
---------------------

The most powerful feature available via Trovi is the ability to re-launch the
available artifacts within Chameleon. Clicking "Launch with JupyterHub" will
open a new Jupyter Notebook server with the artifacts downloaded (we support
artifacts up to 500MB in total size, please contact the |Help Desk| if you need
more space). The animation below shows how easy it is:

.. figure:: sharing/sharing_launching.gif
   :alt: Animation of clicking launch button.
   :figclass: screenshot

   Clicking the "Launch with JupyterHub" button to import a Trovi artifact into
   your own Jupyter server.

Packaging shared artifacts
==========================

You can publish new artifacts to Trovi either from your primary Jupyter server
or by editing a previously-shared artifact. In the latter case, you are
effectively creating a new "forked" artifact owned by you.

When you've finished creating or making changes to an experiment, in the Jupyter
interface, select the directory (not a single file) you wish to package. Then,
click on the "Share" tab and select "Package as a new artifact". Your artifact
is now packaged and uploaded to Chameleon file storage, and you'll be prompted
to fill out descriptions about the artifact. Don't worry if you want to change
this later---you will be able to :ref:`edit them on the Trovi portal or within
Jupyter <trovi-edit>`.

Congratulations! Your artifact is now uploaded to Trovi---but to make it
accessible to others you need to :ref:`adjust its sharing settings
<trovi-sharing>`.

.. figure:: sharing/sharing_packaging.gif
   :alt: Animation of packaging a new artifact from Jupyter.
   :figclass: screenshot

.. _trovi-new-version:

Saving new versions
-------------------

If you make changes to your artifact, you can submit an updated version. Within
Jupyter, you navigate to the "Sharing" tab, but this time you click "Create new
artifact version". The different versions are viewable on the Trovi portal
after clicking on the artifact.

.. figure:: sharing/sharing_new_version.gif
   :alt: Animation of uploading a new artifact version from Jupyter.
   :figclass: screenshot

.. _trovi-edit:

Editing artifacts
-----------------

You can edit an artifact's metadata, including its title, description, and list
of authors at any time via the Jupyter interface.

.. figure:: sharing/sharing_edit_meta.gif
   :alt: Animation of editing an artifact's metadata.
   :figclass: screenshot

This edit view is also available from Trovi via the "Edit" button.

.. _trovi-sharing:

Adjusting sharing settings
--------------------------

When you first upload your packaged artifact to Trovi, its visibility is set as
private, meaning only you can see or launch it. There are multiple options to
change the visibility of the artifact, and you have the option to decide how
visible you want it to be.

1. **Share via private link**: this option allows you to share the experiment to
   select people, like individual colleagues, advisors, or students. Anybody in
   possession of the link can view and launch any version of the artifact.
2. **Share with projects**: this option allows you to share the experiment with
   members of a Chameleon Project. You can also share amongst multiple projects.
3. **Publish with DOI**: this option allows you to :ref:`publish a version of your
   artifact to Zenodo <trovi-zenodo>`.

To make your artifact shareable follow the actions shown in the animation below:
first select how your want to share and then your sharing destination.

.. _trovi-zenodo:

Publishing to Zenodo
^^^^^^^^^^^^^^^^^^^^

Trovi is intended for sharing work in progress with a limited group of "friends
and family". However, once you complete your experiment package you may want to
publish it so that you can reference it from your paper. To do that Chameleon
supports integration with Zenodo, an open-access storage repository backed by
CERN, for permanent artifact hosting. To share your artifact and store it on
Zenodo, go to the "Share" page for the artifact. On the right-hand side you'll
see a list of all versions you've saved. Pick the version you want to publish to
Zenodo and check "Request DOI", then click "Save."

.. important::

   Once published, **Zenodo artifacts cannot be deleted** and are additionally
   **publicly available**. Your artifact will appear in Trovi in the "Public"
   section, and any Chameleon user can access it, as can anybody on the
   Internet via Zenodo's own listing.

This also creates a DOI, which you can easily include in your
paper. The artifacts shared on Zenodo also appear on Trovi.
