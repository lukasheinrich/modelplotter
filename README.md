#modelplotter

extracted stuff from https://github.com/lukasheinrich/modelinspector.cern.ch to be used as a library

### install

    virtualenv venv
    source venv/bin/activate
    pip install -r requirements.txt

### 

    Usage: plot.py fit [OPTIONS] ROOTFILE WORKSPACE OUTPUT

    Usage: plot.py plot_channel [OPTIONS] ROOTFILE WORKSPACE CHANNEL OBSERVABLE
                            PARPOINTFILE

    

### instructions

One can fit a workspace stored in a ROOT file using the `fit` subcommand, and write out the fit result in YAML format

    plot.py fit ~/some/path/to/file.root combined fitresult.yml
     
For any given YAML file with a dictionary specifying the model values the model can be fit via

    plot.py fit ~/some/path/to/file.root combined channel1 x fitresult.yml
