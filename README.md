# 📦 Parsers for Ship Image Collection

This branch contains Jupyter notebooks with parsers developed by our team to collect ship and hydrocycle images. These images are later used to build our custom dataset for the project.

---

## 🧭 Notebooks Overview

This branch includes three main parsers:

- `vesselsfinder_parser.ipynb` — Collects ship images from [vesselfinder.com](https://www.vesselfinder.com)
- `fleetphoto_parser.ipynb` — Parses images and related data from [fleetphoto.ru](https://fleetphoto.ru)
- `istock_hydrocycles_parser.ipynb` — Collects **hydrocycle** images from [istockphoto.com](https://www.istockphoto.com)  
  > Note: We deliberately use the term **Hydrocycles** instead of Jet Ski to reflect a more technical classification.

---

## 🛥️ Dataset Classes

We defined six primary vessel classes to be used in our detection model:

| Class         | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| **Industrial** | Cargo vessels: bulk carriers, container ships, tankers, etc.                |
| **Yacht**       | Yachts of all sizes: from small recreational to large luxury vessels        |
| **Boat**        | Boats, motorboats, speedboats, etc.                                         |
| **Special**     | Support vessels: tugs, icebreakers, fire and technical service ships        |
| **Hydrocycles** | Personal watercrafts. Note: we use the term **Hydrocycles**, not Jet Ski    |
| **Transport**   | Passenger vessels: ferries, riverboats, cruise ships, etc.                  |

---

## 🌐 Data Sources

All images and information were collected exclusively from open and verified sources:

- [vesselfinder.com](https://www.vesselfinder.com)
- [fleetphoto.ru](https://fleetphoto.ru)
- [istockphoto.com](https://www.istockphoto.com)

---

## 📌 Branch Purpose

The purpose of this branch is to automate the collection of vessel images, categorized by type, to build a unique dataset that will be used for annotation and neural network training.

---

## 🛠️ Dependencies

The notebooks use the following libraries:

- selenium, hashlib, os, time, io, PIL, urllib, requests

---

## 🔄 Next Step

Once the parsers are executed and the images are cleaned, the collected data is transferred to the dataset branch for manual/semi-automatic annotation and preparation for training the YOLOv8 model.
