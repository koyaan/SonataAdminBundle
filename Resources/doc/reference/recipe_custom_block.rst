Creating a Custom Block for your Dashboard
==========================================

This recipe is heavily based on this .. _Stackoverflow Response: http://stackoverflow.com/questions/14113259/how-to-add-custom-link-or-button-to-sonataadminbundle-dashboard-in-symfony2

To add a custom block you need to create a new block using Sonata Block Bundle.
The core template ``dashboard.html.twig`` of the SonataAdminBundle iterates over all blocks that are configured
in the ``sonata_admin.dashboard.blocks`` key of your configuration.

Still, Admin Bundle iterates all your entity blocks in the template block_admin_list.html.twig.
Creating your custom block template it is from here that you can take layout to wrap your custom groups (sections)
 and buttons so they have same feel as those of the entities groups.

The recipe
----------

