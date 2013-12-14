Creating a Custom Block for your Dashboard
==========================================

This recipe is heavily based on this .. _Stackoverflow Response: http://stackoverflow.com/questions/14113259/how-to-add-custom-link-or-button-to-sonataadminbundle-dashboard-in-symfony2
`Python <http://www.python.org/>`_

To add a custom block you need to create a new block using Sonata Block Bundle.
The core template ``dashboard.html.twig`` of the SonataAdminBundle iterates over all blocks that are configured
in the ``sonata_admin.dashboard.blocks`` key of your configuration.

SonataAdminBundle decorates all entity blocks with the template ``block_admin_list.html.twig``.
You can use this template as a starting point for your own custom blocks to have the same look and feel.

The recipe
----------

- create a new block class that implements BlockBundleInterface
- create a new block template
- create a block service (read and understand what services are in Symfony 2 Documentation)
- add your newly created service to SonataBlockBundle configuration
- add your newly created service to SonataAdminBundle configuration

