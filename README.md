# EvCamMOKE

This is a public repository of DVS event camera data sets. 

The data in "SlowExpansion" and "Feedback" is used to generate results of our publication "Event-based Vision in Magneto-Optic Kerr Effect Microscopy", which describes details of the experiments. (https://doi.org/10.1063/5.0090714)

The data in "ExtraData" is extra data not in the publication.

# Raw Data Format

The raw data is stored as CSV files. 

Each event forms a line as "x, y, polarity, timestamp" in the CSV file. This is following convention from Prophesee and is different from "timestamp, x, y, polarity" standard established by RPG (https://rpg.ifi.uzh.ch/davis_data.html).

The DVS sensor dimension is 640(H) x 480(V).

polarity=0 means an OFF event (intensity decreasing). polarity=1 means an ON event (intensity increasing).

Timestamps are in microseconds.

Events are sorted with the timestamps so that the timestamps in each CSV file are monotonic.
