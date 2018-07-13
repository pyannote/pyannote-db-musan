# MUSAN plugin for pyannote.database

## Citation

```bibtex
@misc{musan2015,
  author = {David Snyder and Guoguo Chen and Daniel Povey},
  title = {{MUSAN}: {A} {M}usic, {S}peech, and {N}oise {C}orpus},
  year = {2015},
  eprint = {1510.08484},
  note = {arXiv:1510.08484v1}
}
```

## Usage

### Iterating over all background noises:

```python
>>> from pyannote.database import get_protocol
>>> protocol = get_protocol('MUSAN.Collection.BackgroundNoise')
>>> for current_file in protocol.files():
...     # do something with current file
...     pass
```

### Other files

Replacing `BackgroundNoise` with `Noise` will iterate over all noises.
One can also use `Speech` or `Music` subsets.
