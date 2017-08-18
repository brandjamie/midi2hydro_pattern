# midi2hydro_pattern

The script converts general midi drum patterns (which can be found easily online) to hydrogen pattern format. 
When installed to the hydrogen patterns directory (usually '~/.hydrogen/data/patterns') the patterns are automaticcaly imported to the hydrogen library. 

## Installation

The script requires the python_midi library which can be installed through pip:

```pip install git+https://github.com/vishnubob/python-midi@feature/python3```

## Usage

The script accepts four parameters: the input filename, 
                                    the output filename, 
                                    the category (as it appears in the hydrogen library),
                                    the name (as it appears in the hydrogen library)

``` python midi2hydro_pattern.py "my_midi_file.mid" "my_h2_pattern.h2pattern" "pattern_genre" "pattern_name" ```

If only the input filename is provided, the other parameters will be created from it. 

``` python midi2hydro_pattern.py "my_midi_file.mid"```

