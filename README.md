armada-heal
===========

Script for healing overloaded armada ship.

It works in 4 phases:
1. Preventing services from registering to consul catalog to decrease consul load.
2. Restarting consul.
3. Sleep phase to let consul catch up.
4. Allowing services to register to consul back again.

All steps are executed on current ship only.

Installation:
```
pip install armada-heal
```

To run type:
```
armada-heal
```

Upload new version to PyPI:
```
python setup.py register sdist upload
```
