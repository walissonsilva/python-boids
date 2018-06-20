# pyboids

This is a port of Peter Keller's sample boids program to python3.

For the original Common Lisp version of boids, check out:
[Boids Flocking Model](http://pages.cs.wisc.edu/~psilord/lisp-public/boids.html)

_NOTE:_ This port was taken from an earlier, unpublished snapshot
of the Common Lisp version and is now somewhat out of date.

## Background (from Peter Keller)

This is a _naive_ boids implementation derived from this paper:

http://www.cs.toronto.edu/~dt/siggraph97-course/cwr87/

The boids exist in a 3D cube which is a hypertorus. However, the neighborhood
equations in the vector math does not take that geometry into consideration.
Visually, the error is negligible.

The various nasty constants found in the method implementations of the
correction protocol are mostly due to not completing the physics all the way to
dealing with boid mass and volume and for visual effect of what I thought
looked nice.

## Dependencies

* python3
  Debian: python3-all-dev
  http://wiki.python.org/moin/Python2orPython3

* pygame
  Debian: python3-pygame
  http://www.pygame.org/wiki/FrequentlyAskedQuestions#Does%20Pygame%20work%20with%20Python%203?

* python-opengl
  Debian: Currently not supported for python3 in Debian unstable, build from source with
    --prefix /usr/local
    http://packages.debian.org/search?keywords=python-opengl&searchon=names&suite=all&section=all
  http://pyopengl.sourceforge.net/
  https://code.launchpad.net/pyopengl

## Running

To try it out yourself, clone this and run:

```
./boids.py
```

## Contributors

* pkeller
* tmarble

## License

This project is licensed under the permissive [MIT](http://opensource.org/licenses/MIT) license
