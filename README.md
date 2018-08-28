# Open Research Bases

This is the future home of the [Open Research Bases](https://openbases.github.io) 
Group! We create template bases for the [Open Journals](https://www.github.com/openjournals)
organization of journals to drive reproducible, automated research and software
development.

![img/openbases-petri.png](img/openbases-petri.png)

## Resources

 - [Open Journals](https://www.github.com/openjournals)
 - [The Experiment Factory](https://expfactory.github.io)
 - [LabJS](https://labjs.readthedocs.io)
 - [JsPsych](https://www.jspsych.org/)
 - [Robots](https://github.com/expfactory/expfactory-robots)

## Templates

> Where are the bases?

We are putting together the first toy examples that will put together a selection of components from above
to generate a fully reproducible generation to publication pipeline! Stay tuned.

## Development

I'll put notes here until I'm comfortable with these technologies! We use [mkdocs](https://www.mkdocs.org) because it's  easy to write markdown files. Specifically, we are using the [material](https://squidfunk.github.io/mkdocs-material/) theme.

### Local
Here are the dependencies you should install:

```
pip install mkdocs mkdocs-material click-man markdown-include
```

The resulting docs will be built from [src](src) into [docs](docs). The build and serve happens
like this!

```
mkdocs serve
```

Then open your browser to [http://127.0.0.1:8000](http://127.0.0.1:8000)

### Mkdocs Quick Reference

#### Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

#### Project layout

```bash
    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
```

### Docker
If you want, you can also develop in the container!

```
docker build -t openbases/openbases.github.io .
docker run --rm -v --port 8000:8000 $PWD/:/code openbases/openbases.github.io
```

## Support

Please don't hesitate to reach out and 
[ask us a question](https://www.github.com/openbases/openbases.github.io/issues), 
or contribute!
