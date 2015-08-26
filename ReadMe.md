## Fabric8 Development Projects

This project creates OpenShift projects (kubernetes namespaces) for the main GitHub repositories used by the fabric8 team to build fabric8 itself.

This then allows you to view the different projects in the [fabric8 console](http://fabric8.io/guide/console.html) (in the `Projects` -> `Builds` section) and easily switch between different namespaces (e.g. `team-fabric8` or `team-hawtio`) and for each namespace see all the individual github repositories and easily navigate to their repository, commits, issues, chat room, jenkins builds, tags and so forth.

Over time this UI should improve to include nice developer dashboards so its easier to view different the activities on groups of github projects in a single browser page together with to provide better UI integration between the [CI / CD flows](http://fabric8.io/guide/cdelivery.html) and the underlying github repositories.

### Creating the Development Projects in OpenShift

If you have a running [Fabric8 installation on OpenShift](http://fabric8.io/guide/getStarted/vagrant.html) then just run:

    mvn fabric8:apply-projects

and all the projects will be imported into OpenShift for viewing in the Fabric8 console
