import numpy as np

import sqlalchemy
from sqlalchemy.ext.automap import automap_base
from sqlalchemy.orm import Session
from sqlalchemy import create_engine, func

from flask import Flask, jsonify

engine = create_engine("sqlite:///Resources/hawaii.sqlite")

# reflect an existing database into a new model
Base = automap_base()
# reflect the tables
Base.prepare(engine, reflect=True)

# Save reference to the table
Measurements = Base.classes.measurement

# Create our session (link) from Python to the DB
session = Session(engine)

app = Flask(__name__)

@app.route("/")
def welcome ():
    "List all available api route."
    return (
    f"Available Routes:<br/>"
    f"/api/measurement<br/>"
    f"/api/stations"
    )

@app.route("/api/station")
def station():
    """Return a list of all stations"""
    #Query
    results = session.query(measurement.station).all()
    #covert tuples into list
    stations = list(np.ravel(results))

    return jsonify(stations)

@app.route("/api/measurement")
def measurement():
    """Return a list of all precipitations and dates"""
    #Query
    results = session.query(Measurements.station, Measurements.prcp, Measurements.date, Measurements.tobs).all()
    #covert tuples into list
    measurements = []
    for prcp in results:
        measurements_dict = {}
        measurements_dict["station"] = station
        measurements_dict["prcp"] = prcp
        measurements_dict["date"] = date
        measurements_dict["tobs"] = tobs
    
    return jsonify(measurements)

if __name__ == '__main__':
    app.run(debug=True)