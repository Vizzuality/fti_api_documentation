# AnnexOperators

## How obtain all annex_operators

To obtain all annex_operators:

```shell
curl -X GET http://localhost:3000/annex_operators \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>

> Example response:

```json
{
  "data": [
    {
      "id": "42",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Abandon de bois",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "45",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "225",
              "type": "severities"
            },
            {
              "id": "226",
              "type": "severities"
            },
            {
              "id": "227",
              "type": "severities"
            },
            {
              "id": "228",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "65",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "1",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Abandonment of timber ",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "1",
              "type": "severities"
            },
            {
              "id": "4",
              "type": "severities"
            },
            {
              "id": "3",
              "type": "severities"
            },
            {
              "id": "2",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "202",
              "type": "laws"
            },
            {
              "id": "203",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "34",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Company not registered according to regulations",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "135",
              "type": "severities"
            },
            {
              "id": "136",
              "type": "severities"
            },
            {
              "id": "133",
              "type": "severities"
            },
            {
              "id": "134",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "4",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "6",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting outside permit boundaries",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "23",
              "type": "severities"
            },
            {
              "id": "22",
              "type": "severities"
            },
            {
              "id": "21",
              "type": "severities"
            },
            {
              "id": "24",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "23",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "8",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting trees below minimum diameter",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "31",
              "type": "severities"
            },
            {
              "id": "32",
              "type": "severities"
            },
            {
              "id": "30",
              "type": "severities"
            },
            {
              "id": "29",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "5",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "7",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Cutting trees below minimum diameter",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "28",
              "type": "severities"
            },
            {
              "id": "27",
              "type": "severities"
            },
            {
              "id": "26",
              "type": "severities"
            },
            {
              "id": "25",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "11",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Default on demarcation of cutting permit boundaries",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "43",
              "type": "severities"
            },
            {
              "id": "41",
              "type": "severities"
            },
            {
              "id": "42",
              "type": "severities"
            },
            {
              "id": "44",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "191",
              "type": "laws"
            },
            {
              "id": "192",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "12",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Default on fine payments",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "48",
              "type": "severities"
            },
            {
              "id": "47",
              "type": "severities"
            },
            {
              "id": "46",
              "type": "severities"
            },
            {
              "id": "45",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "3",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": []
        }
      }
    },
    {
      "id": "14",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Default on maintenance of exploitation documents",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "54",
              "type": "severities"
            },
            {
              "id": "53",
              "type": "severities"
            },
            {
              "id": "56",
              "type": "severities"
            },
            {
              "id": "55",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "30",
              "type": "laws"
            }
          ]
        }
      }
    },
    {
      "id": "10",
      "type": "annex_operators",
      "attributes": {
        "illegality": "Default on markings on logs, stumps, other wood products",
        "details": null
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        },
        "severities": {
          "data": [
            {
              "id": "40",
              "type": "severities"
            },
            {
              "id": "39",
              "type": "severities"
            },
            {
              "id": "37",
              "type": "severities"
            },
            {
              "id": "38",
              "type": "severities"
            }
          ]
        },
        "categories": {
          "data": [
            {
              "id": "6",
              "type": "categories"
            }
          ]
        },
        "comments": {
          "data": []
        },
        "laws": {
          "data": [
            {
              "id": "186",
              "type": "laws"
            },
            {
              "id": "188",
              "type": "laws"
            },
            {
              "id": "187",
              "type": "laws"
            }
          ]
        }
      }
    }
  ],
  "included": [
    {
      "id": "45",
      "type": "countries",
      "attributes": {
        "iso": "CMR",
        "region_iso": "MA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            6,
            12.5
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            0.618107263658459,
            19.464922564119
          ]
        },
        "is_active": true,
        "name": "Cameroon",
        "region_name": "Middle Africa"
      }
    },
    {
      "id": "225",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": "Not specified"
      }
    },
    {
      "id": "226",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": "Not specified"
      }
    },
    {
      "id": "227",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": "Not specified"
      }
    },
    {
      "id": "228",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": "Not specified"
      }
    },
    {
      "id": "6",
      "type": "categories",
      "attributes": {
        "name": "Timber harvesting"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "1",
              "type": "annex_governances"
            },
            {
              "id": "2",
              "type": "annex_governances"
            },
            {
              "id": "4",
              "type": "annex_governances"
            },
            {
              "id": "5",
              "type": "annex_governances"
            },
            {
              "id": "6",
              "type": "annex_governances"
            },
            {
              "id": "7",
              "type": "annex_governances"
            },
            {
              "id": "8",
              "type": "annex_governances"
            },
            {
              "id": "10",
              "type": "annex_governances"
            },
            {
              "id": "11",
              "type": "annex_governances"
            },
            {
              "id": "14",
              "type": "annex_governances"
            },
            {
              "id": "15",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "7",
              "type": "annex_operators"
            },
            {
              "id": "26",
              "type": "annex_operators"
            },
            {
              "id": "36",
              "type": "annex_operators"
            },
            {
              "id": "32",
              "type": "annex_operators"
            },
            {
              "id": "41",
              "type": "annex_operators"
            },
            {
              "id": "42",
              "type": "annex_operators"
            },
            {
              "id": "8",
              "type": "annex_operators"
            },
            {
              "id": "31",
              "type": "annex_operators"
            },
            {
              "id": "19",
              "type": "annex_operators"
            },
            {
              "id": "18",
              "type": "annex_operators"
            },
            {
              "id": "5",
              "type": "annex_operators"
            },
            {
              "id": "10",
              "type": "annex_operators"
            },
            {
              "id": "30",
              "type": "annex_operators"
            },
            {
              "id": "25",
              "type": "annex_operators"
            },
            {
              "id": "4",
              "type": "annex_operators"
            },
            {
              "id": "6",
              "type": "annex_operators"
            },
            {
              "id": "11",
              "type": "annex_operators"
            },
            {
              "id": "14",
              "type": "annex_operators"
            },
            {
              "id": "17",
              "type": "annex_operators"
            },
            {
              "id": "15",
              "type": "annex_operators"
            },
            {
              "id": "2",
              "type": "annex_operators"
            },
            {
              "id": "1",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "65",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": "Article 158 de la loi de 1994",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "7",
      "type": "countries",
      "attributes": {
        "iso": "COD",
        "region_iso": "MA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -2.5,
            23.5
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            0.618107263658459,
            19.464922564119
          ]
        },
        "is_active": true,
        "name": "Democratic Republic of the Congo",
        "region_name": "Middle Africa"
      }
    },
    {
      "id": "1",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "4",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "3",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "2",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "202",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": "Art.65 de l'arrêté 050 au point 6 (Valable depuis 2015 jusqu'à octobre 2016)-Art. 42 point 5 arrêté interministériel 035/2006 (valable de 2006-2015)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "203",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " Article 64 point 6 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre (valable depuis octobre 2016)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "135",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "136",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "133",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "134",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "4",
      "type": "categories",
      "attributes": {
        "name": "Right to exploit"
      },
      "relationships": {
        "annex_governances": {
          "data": []
        },
        "annex_operators": {
          "data": [
            {
              "id": "34",
              "type": "annex_operators"
            },
            {
              "id": "35",
              "type": "annex_operators"
            },
            {
              "id": "21",
              "type": "annex_operators"
            },
            {
              "id": "22",
              "type": "annex_operators"
            },
            {
              "id": "20",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "23",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "22",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "21",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "24",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "23",
      "type": "laws",
      "attributes": {
        "vpa_indicator": "Not applicable",
        "legal_reference": "Art. 65 de l’arrêté 050/2015 point 1 (Valable depuis 2015)-Art 42 de l'arrêté 035/2016 (Valable jusqu'en 2015)-Article 64 point 1 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre -valable depuis octobre 2016)",
        "legal_penalty": "Art 143. Servitude pénale de trois mois à deux ans et d’une amende allant de 20 000 à 100 000 FC"
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "47",
      "type": "countries",
      "attributes": {
        "iso": "COG",
        "region_iso": "MA",
        "country_centroid": {
          "type": "Point",
          "coordinates": [
            -1,
            15.5
          ]
        },
        "region_centroid": {
          "type": "Point",
          "coordinates": [
            0.618107263658459,
            19.464922564119
          ]
        },
        "is_active": true,
        "name": "Congo",
        "region_name": "Middle Africa"
      }
    },
    {
      "id": "31",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "32",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "30",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "29",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "5",
      "type": "laws",
      "attributes": {
        "vpa_indicator": "4.6.1: L’entreprise respecte les essences à prélever, les diamètres d’abattage et le volume à prélever, fixés par les textes réglementaires et le plan d’aménagement.",
        "legal_reference": "Décret 2002-437 Art.91",
        "legal_penalty": "Amende de 20 000 à 5 000 000 FCFA et emprisonnement maximum de 3 mois ou l'une de ces 2 peines seulement"
      },
      "relationships": {
        "country": {
          "data": {
            "id": "47",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "28",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "27",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "26",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "25",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "43",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "41",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "42",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "44",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "191",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": "Art. 5 alinéa  4 de l' arrêté interministériel 011/2007 (abrogé en 2015) -Art. 15 de l’Arrêté n° 036/2006 du 05 octobre 2006 (abrogé en 2015)-Art 14 de l'arrêté 034/2015 (valable depuis juillet 2015)-Art 13 arrêté 028/2008 fixant les modèles de contrat de concession forestière",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "192",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " Article 58 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre -valable depuis octobre 2016)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "48",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "47",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "46",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "45",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "3",
      "type": "categories",
      "attributes": {
        "name": "Payments"
      },
      "relationships": {
        "annex_governances": {
          "data": [
            {
              "id": "12",
              "type": "annex_governances"
            },
            {
              "id": "13",
              "type": "annex_governances"
            }
          ]
        },
        "annex_operators": {
          "data": [
            {
              "id": "12",
              "type": "annex_operators"
            },
            {
              "id": "28",
              "type": "annex_operators"
            },
            {
              "id": "13",
              "type": "annex_operators"
            }
          ]
        }
      }
    },
    {
      "id": "54",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "53",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "56",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "55",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "30",
      "type": "laws",
      "attributes": {
        "vpa_indicator": "Not applicable",
        "legal_reference": "Art. 50 et 60-61 (declarations) de l’arrêté 035/2006 (valide jusqu'en 2015)-Articles 69-79 de l'arrêté 050/2015 relatif à l'exploitation forestière",
        "legal_penalty": "Art 143. Servitude pénale de trois mois à deux ans et d’une amende allant de 20 000 à 100 000 FC"
      },
      "relationships": {
        "country": {
          "data": {
            "id": "7",
            "type": "countries"
          }
        }
      }
    },
    {
      "id": "40",
      "type": "severities",
      "attributes": {
        "level": 0,
        "details": null
      }
    },
    {
      "id": "39",
      "type": "severities",
      "attributes": {
        "level": 1,
        "details": null
      }
    },
    {
      "id": "37",
      "type": "severities",
      "attributes": {
        "level": 3,
        "details": null
      }
    },
    {
      "id": "38",
      "type": "severities",
      "attributes": {
        "level": 2,
        "details": null
      }
    },
    {
      "id": "186",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": "Art.s 6",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "188",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 49 arrêté 035/2006 (abrogé en 2015)-Article 66 de l'arrêté 084/2016 portant conditions et règles d'exploitation de bois d'oeuvre -valable depuis octobre 2016)",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    },
    {
      "id": "187",
      "type": "laws",
      "attributes": {
        "vpa_indicator": null,
        "legal_reference": " 68 l’arrêté ministériel N°050/2015 (valable depuis septembre 2015)-article 48",
        "legal_penalty": null
      },
      "relationships": {
        "country": {
          "data": null
        }
      }
    }
  ],
  "links": {
    "first": "http://otp-staging.ipq.co/annex_operators?page%5Bnumber%5D=1",
    "prev": "http://otp-staging.ipq.co/annex_operators?page%5Bnumber%5D=1",
    "next": "http://otp-staging.ipq.co/annex_operators?page%5Bnumber%5D=2&page%5Bsize%5D=10",
    "last": "http://otp-staging.ipq.co/annex_operators?page%5Bnumber%5D=5&page%5Bsize%5D=10",
    "self": "http://otp-staging.ipq.co/annex_operators?page%5Bnumber%5D=1&page%5Bsize%5D=10"
  },
  "meta": {
    "total_items": 42
  }
}
```

### Pagination params

| Field           | Description                | Type
| -------------   |:-------------:| -----:|
| page[size]      | Number elements per page   | Number
| page[number]    | Number of page             | Number

> Return the annex_operators of the page 2 with 5 elements per page

```shell
curl -X GET http://localhost:3000/annex_operators?page[size]=5&page[number]=2
```

### Filter params

Available filters:

| Field         | Description           | Type
| ------------- |:-------------:| -----:|
| sort          | Sort json response by specific attributes (illegality, created_at, updated_at) | Text
| country       | Filter by country ID | Integer


> To obtain all annex_operators sorted by illegality:

```shell
curl -X GET http://localhost:3000/annex_operators?sort=illegality \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

```shell
curl -X GET http://localhost:3000/annex_operators?sort=-illegality \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

> To filter annex_operators by specific country:

```shell
curl -X GET http://localhost:3000/annex_operators?country=<country-id> \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

## How to obtain specific annex_operator

To obtain specific annex_operator:

```shell
curl -X GET http://localhost:3000/annex_operators/33 \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="success">
Remember — the response is jsonapi format
</aside>


## Creating a AnnexOperator

In order to create a annex_operator, you need an authorization token for current admin.

Only admin should be able to create AnnexOperators

To create a annex_operator, you need to define all of the required fields in the request body. The fields that compose a annex_operator are:

| Field               | Description                                                   | Type   | Values                                          | Required |
| ------------------  | -------------------------------------------------------------:| ------:| -----------------------------------------------:|  -------:|
| illegality          | Name of the illegality                                        | Text    | Any Text                                        | Yes
| country_id          | ID of country                                                 | Integer | Any Text                                        | No
| details             | Datails - description                                         | Text    | Any Text                                        | No
| category_ids        | ID's of categories                                            | Array   | Valid category ids                              | No
| law_ids             | ID's of laws                                                  | Array   | Valid law ids                                   | No
| severities_attributes | Nested severities attributes. Sample: "severities_attributes": [{ "level": 2, "details": "Lorem ipsum" }, { "id": 2, "details": "Lorem ipsum update details for severity id 2" }]                               | Array   | Valid array of object (Severity)    | No

> To create a annex_operator, you have to do a POST with the following body:

```shell
curl -X POST http://localhost:3000/annex_operators \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json" -d \
'{__
  "annex_operator": {
      "illegality": "Art. 100",
      "details": "Problem",
      "severities_attributes": [{ "level": 2, "details": "Lorem ipsum" }, { "id": 2, "details": "Lorem ipsum update details for severity id 2" }],
      more attributes...
  }
}'
```
<aside class="notice">
  Remember that create annex_operator is an authenticated endpoint!
</aside>


## Updating a AnnexOperator

In order to modify the annex_operator, you can PUT/PATCH a request.
It accepts the same parameters as the _create annex_operator_ endpoint, and you will need an authentication token.

> An example update request:

```shell
curl -X PATCH http://localhost:3000/annex_operators/<annex_operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"  -d \
'{__
  "annex_operator": {
      "illegality": "Another illegality for the annex_operator"
  }
}'
```

<aside class="notice">
Remember — create annex_operator is an authenticated endpoint!
</aside>

## Deleting a AnnexOperator
You can delete a annex_operator! Just send a DELETE request to the endpoint:

```shell
curl -X DELETE http://localhost:3000/annex_operators/<annex_operator-id> \
-H "Authorization: Bearer <your-token>" \
-H "OTP-API-KEY: Bearer <your-api-key>" \
-H "Content-Type: application/json"
```

<aside class="notice">
Remember — create annex_operator is an authenticated endpoint!
</aside>
