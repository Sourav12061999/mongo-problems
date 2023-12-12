### Problem Description

## Given below ecommerse users json data to perform mongo queries.

```
[
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190bb"
    },
    "st": "x+60900-005300",
    "ts": {
      "$date": "1984-03-05T15:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-5.3, 60.9]
    },
    "elevation": 9999,
    "callLetters": "TFRB",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 7.5,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1018.5,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 220,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 12.3,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 4000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MW1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 3,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "08",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "99",
        "quality": "9"
      },
      "lowCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ]
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190df"
    },
    "st": "x+21900-072800",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-72.8, 21.9]
    },
    "elevation": 9999,
    "callLetters": "99999",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 999.9,
      "quality": "9"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1017.9,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 80,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 10,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "GF1", "MD1", "SA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "05",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "05",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 800,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "05",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "00",
        "quality": "1"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "7",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0.2,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "seaSurfaceTemperature": {
      "value": 26,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 8,
        "height": 3,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190cd"
    },
    "st": "x+55300+005000",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [5, 55.3]
    },
    "elevation": 9999,
    "callLetters": "SHIP",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 6.7,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1032,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 290,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 7.2,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 10000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MW1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "03",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "00",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "05",
        "quality": "1"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ]
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190b8"
    },
    "st": "x+47600-047900",
    "ts": {
      "$date": "1984-03-05T13:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-47.9, 47.6]
    },
    "elevation": 9999,
    "callLetters": "VCSZ",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": -3.1,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1015.3,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 999,
        "quality": "9"
      },
      "type": "9",
      "speed": {
        "rate": 999.9,
        "quality": "9"
      }
    },
    "visibility": {
      "distance": {
        "value": 999999,
        "quality": "9"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 999
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190c3"
    },
    "st": "x+56500+002100",
    "ts": {
      "$date": "1984-03-05T15:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [2.1, 56.5]
    },
    "elevation": 9999,
    "callLetters": "PLAT",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 7.1,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1028.2,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 320,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 4.1,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "OA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 3,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "00",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "00",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "00",
        "quality": "1"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "2",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0.4,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 5,
        "height": 0.5,
        "quality": "9"
      },
      "seaState": {
        "code": "00",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190d7"
    },
    "st": "x+12800+114300",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [114.3, 12.8]
    },
    "elevation": 9999,
    "callLetters": "VSBE",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 25,
      "quality": "1"
    },
    "dewPoint": {
      "value": 24.4,
      "quality": "1"
    },
    "pressure": {
      "value": 1010.7,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 30,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 7.7,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "1",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "01",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "99",
        "quality": "9"
      },
      "lowCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "0",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0.8,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ]
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190c0"
    },
    "st": "x+59500+001500",
    "ts": {
      "$date": "1984-03-05T15:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [1.5, 59.5]
    },
    "elevation": 9999,
    "callLetters": "PLAT",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 6.3,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1026.1,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 280,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 9.3,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 10000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MW1", "OA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 3,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "07",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "99",
        "quality": "9"
      },
      "lowCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "lowestCloudBaseHeight": {
        "value": 1250,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 99,
        "height": 2.5,
        "quality": "9"
      },
      "seaState": {
        "code": "00",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190e0"
    },
    "st": "x+54100+010800",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [10.8, 54.1]
    },
    "elevation": 9999,
    "callLetters": "SHIP",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 5.5,
      "quality": "1"
    },
    "dewPoint": {
      "value": 2.2,
      "quality": "1"
    },
    "pressure": {
      "value": 1026.5,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 280,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 5.1,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 10000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MW1", "SA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "1",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "4",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "00",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "00",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "00",
        "quality": "1"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "01",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": 1.6,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 1,
        "height": 0,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190eb"
    },
    "st": "x+26400-076000",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-76, 26.4]
    },
    "elevation": 9999,
    "callLetters": "UWTZ",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 24.2,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1018.4,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 90,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 13,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "SA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "1",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "04",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "04",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "01",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 450,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "01",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "00",
        "quality": "1"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "4",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": 26,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 4,
        "height": 3,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151190f4"
    },
    "st": "x-01100+151500",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [151.5, -1.1]
    },
    "elevation": 9999,
    "callLetters": "GZSH",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 25.3,
      "quality": "1"
    },
    "dewPoint": {
      "value": 24.3,
      "quality": "1"
    },
    "pressure": {
      "value": 1006.4,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 230,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 4.6,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 210,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "SA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "0",
      "estimatedWaterDepth": 999
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "8",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "05",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "05",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "02",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 250,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "7",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0.8,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "25",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": 29,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 4,
        "height": 1,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf715119381"
    },
    "st": "x+54600-137200",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-137.2, 54.6]
    },
    "elevation": 9999,
    "callLetters": "WNDO",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 5,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1020.5,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 110,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 9.3,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 420,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "SA1", "UA1", "UG1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "2",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "08",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "08",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "05",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 450,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "7",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 1.5,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": 8.3,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 3,
        "height": 1.5,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf71511938b"
    },
    "st": "x+49400-064600",
    "ts": {
      "$date": "1984-03-05T18:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-64.6, 49.4]
    },
    "elevation": 9999,
    "callLetters": "ZCKE",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": -3.4,
      "quality": "1"
    },
    "dewPoint": {
      "value": -5.7,
      "quality": "1"
    },
    "pressure": {
      "value": 1022.3,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 290,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 5.1,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "SA1", "UA1", "WD1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 6,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "07",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "00",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "lowestCloudBaseHeight": {
        "value": 450,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "4",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": -1.5,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 0,
        "height": 0,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151193c4"
    },
    "st": "x+63300-016700",
    "ts": {
      "$date": "1984-03-05T21:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-16.7, 63.3]
    },
    "elevation": 9999,
    "callLetters": "TFWI",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 5.2,
      "quality": "1"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 1010.3,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 270,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 19,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 10000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MW1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 0
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 3,
          "quality": "1"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "08",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "99",
        "quality": "9"
      },
      "lowCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "lowestCloudBaseHeight": {
        "value": 1750,
        "quality": "1"
      },
      "midCloudGenus": {
        "value": "99",
        "quality": "9"
      },
      "highCloudGenus": {
        "value": "99",
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ]
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf7151193ff"
    },
    "st": "x+06800+116200",
    "ts": {
      "$date": "1984-03-05T22:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [116.2, 6.8]
    },
    "elevation": 9999,
    "callLetters": "SSUR",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 999.9,
      "quality": "9"
    },
    "dewPoint": {
      "value": 999.9,
      "quality": "9"
    },
    "pressure": {
      "value": 9999.9,
      "quality": "9"
    },
    "wind": {
      "direction": {
        "angle": 999,
        "quality": "9"
      },
      "type": "9",
      "speed": {
        "rate": 999.9,
        "quality": "9"
      }
    },
    "visibility": {
      "distance": {
        "value": 999999,
        "quality": "9"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 99999,
        "quality": "9",
        "determination": "9"
      },
      "cavok": "N"
    },
    "sections": ["AG1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 999
    }
  },
  {
    "_id": {
      "$oid": "5553a998e4b02cf715119402"
    },
    "st": "x+38400-125000",
    "ts": {
      "$date": "1984-03-05T23:00:00.000Z"
    },
    "position": {
      "type": "Point",
      "coordinates": [-125, 38.4]
    },
    "elevation": 9999,
    "callLetters": "BLHW",
    "qualityControlProcess": "V020",
    "dataSource": "4",
    "type": "FM-13",
    "airTemperature": {
      "value": 25.5,
      "quality": "1"
    },
    "dewPoint": {
      "value": 22.1,
      "quality": "1"
    },
    "pressure": {
      "value": 1020,
      "quality": "1"
    },
    "wind": {
      "direction": {
        "angle": 140,
        "quality": "1"
      },
      "type": "N",
      "speed": {
        "rate": 5.1,
        "quality": "1"
      }
    },
    "visibility": {
      "distance": {
        "value": 20000,
        "quality": "1"
      },
      "variability": {
        "value": "N",
        "quality": "9"
      }
    },
    "skyCondition": {
      "ceilingHeight": {
        "value": 22000,
        "quality": "1",
        "determination": "C"
      },
      "cavok": "N"
    },
    "sections": ["AG1", "AY1", "GF1", "MD1", "MW1", "SA1", "UA1"],
    "precipitationEstimatedObservation": {
      "discrepancy": "2",
      "estimatedWaterDepth": 999
    },
    "pastWeatherObservationManual": [
      {
        "atmosphericCondition": {
          "value": "0",
          "quality": "1"
        },
        "period": {
          "value": 99,
          "quality": "9"
        }
      }
    ],
    "skyConditionObservation": {
      "totalCoverage": {
        "value": "01",
        "opaque": "99",
        "quality": "1"
      },
      "lowestCloudCoverage": {
        "value": "01",
        "quality": "1"
      },
      "lowCloudGenus": {
        "value": "00",
        "quality": "1"
      },
      "lowestCloudBaseHeight": {
        "value": 99999,
        "quality": "9"
      },
      "midCloudGenus": {
        "value": "02",
        "quality": "1"
      },
      "highCloudGenus": {
        "value": "06",
        "quality": "1"
      }
    },
    "atmosphericPressureChange": {
      "tendency": {
        "code": "4",
        "quality": "1"
      },
      "quantity3Hours": {
        "value": 0,
        "quality": "1"
      },
      "quantity24Hours": {
        "value": 99.9,
        "quality": "9"
      }
    },
    "presentWeatherObservationManual": [
      {
        "condition": "02",
        "quality": "1"
      }
    ],
    "seaSurfaceTemperature": {
      "value": 13,
      "quality": "9"
    },
    "waveMeasurement": {
      "method": "M",
      "waves": {
        "period": 4,
        "height": 0.5,
        "quality": "9"
      },
      "seaState": {
        "code": "99",
        "quality": "9"
      }
    }
  }
]

```

## Problem Statement

- Find the High pressure and Low pressure Poient accordingly along with co-ordinates as key names "coordinates" and "pressure" ?

- hint - use MongoDB aggregation pipeline with [$match](https://www.mongodb.com/docs/manual/reference/operator/aggregation/match/) & [$project](https://www.mongodb.com/docs/v6.0/reference/operator/aggregation/project/) &  [$sort](https://www.mongodb.com/docs/v6.0/reference/operator/aggregation/sort/) 
 - total data count is 15.
 - [toArray](https://www.mongodb.com/docs/manual/reference/method/cursor.toArray/)
 - can use javaScript Method for the final reasult.


- output should look lke this.

```
[
  {
    coordinates: [ 116.2, 6.8 ],
    pressure: 9999.9
  },
  {
    coordinates: [ 151.5, -1.1 ],
    pressure: 1006.4
  }
]

```
