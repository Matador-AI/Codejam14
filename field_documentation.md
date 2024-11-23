# Vehicle Database Field Documentation

This document provides detailed information about each field in the vehicle dataset.

## Basic Information Fields

### Type
- **Description**: Indicates whether the vehicle is new or used
- **Possible Values**: "New" or "Used"
- **Format**: String
- **Example**: "New"

### Stock
- **Description**: Unique dealer stock number for inventory tracking
- **Format**: Letter followed by 6 digits (LDDDDDD)
- **Example**: "T237890"

### VIN
- **Description**: Vehicle Identification Number, unique identifier for each vehicle
- **Format**: 17-character string following standard VIN format
- **Example**: "A9FGFF8ST43CEFJ3Y"

### Year
- **Description**: Manufacturing year of the vehicle
- **Format**: 4-digit integer
- **Range**: 1900-present
- **Example**: 2024

### Make
- **Description**: Manufacturer/brand of the vehicle
- **Format**: String
- **Example**: "Toyota", "Ford", "BMW"

### Model
- **Description**: Specific model name of the vehicle
- **Format**: String
- **Example**: "Camry", "F-150", "X5"

### Body
- **Description**: Body style/type of the vehicle
- **Format**: String
- **Example**: "Sport Utility", "Sedan", "Pickup Truck"

### ModelNumber
- **Description**: Internal model code combining make and model information
- **Format**: MMPP-LL###L (MM=Make, PP=Model Prefix, L=Letter, #=Number)
- **Example**: "TOCY-AB123X"

## Physical Characteristics

### Doors
- **Description**: Number of doors on the vehicle
- **Format**: Integer
- **Example**: 4

### ExteriorColor
- **Description**: Full name/description of exterior paint color
- **Format**: String
- **Example**: "Snowflake White Pearl Mica"

### InteriorColor
- **Description**: Color of the interior upholstery/trim
- **Format**: String
- **Example**: "Black", "Tan"

### Ext_Color_Generic
- **Description**: Simplified/generic name of exterior color
- **Format**: String
- **Example**: "White", "Red"

### Ext_Color_Code
- **Description**: Manufacturer's color code
- **Format**: String
- **Example**: "25D"

### ExtColorHexCode
- **Description**: Hex color code for exterior color
- **Format**: 6-character hex code
- **Example**: "E7E8E8"

### Int_Color_Generic
- **Description**: Simplified/generic name of interior color
- **Format**: String
- **Example**: "Black"

### Int_Color_Code
- **Description**: Manufacturer's interior color code
- **Format**: String
- **Example**: "TC5"

### Int_Upholstery
- **Description**: Type and material of interior upholstery
- **Format**: String
- **Example**: "Leather", "Cloth"

## Engine and Performance

### EngineCylinders
- **Description**: Number of cylinders in the engine
- **Format**: Integer
- **Example**: 4, 6, 8

### EngineDisplacement
- **Description**: Engine size in liters
- **Format**: String with "L" suffix
- **Example**: "2.5 L"

### EngineDisplacementCubicInches
- **Description**: Engine displacement in cubic inches
- **Format**: Integer
- **Example**: 152

### Engine_Block_Type
- **Description**: Configuration of the engine block
- **Format**: String
- **Example**: "I" (Inline), "V" (V-shaped)

### Engine_Aspiration_Type
- **Description**: Method of air intake for the engine
- **Format**: String
- **Example**: "Turbocharged", "Naturally Aspirated"

### Engine_Description
- **Description**: Detailed description of the engine specifications
- **Format**: String
- **Example**: "Intercooled Turbo Regular Unleaded I-4 2.5 L/152"

### Transmission
- **Description**: Type of transmission system
- **Format**: String
- **Example**: "Automatic", "Manual"

### Transmission_Speed
- **Description**: Number of speeds/gears in the transmission
- **Format**: Integer
- **Example**: 6, 8

### Transmission_Description
- **Description**: Detailed description of the transmission system
- **Format**: String
- **Example**: "6-Speed Automatic w/OD"

### Drivetrain
- **Description**: Type of drive system
- **Format**: String
- **Example**: "AWD", "FWD", "RWD"

### Fuel_Type
- **Description**: Type of fuel the vehicle uses
- **Format**: String
- **Example**: "Gasoline Fuel", "Diesel Fuel"

## Performance Metrics

### CityMPG
- **Description**: EPA estimated city fuel economy
- **Format**: Integer
- **Example**: 20

### HighwayMPG
- **Description**: EPA estimated highway fuel economy
- **Format**: Integer
- **Example**: 26

### EPAClassification
- **Description**: EPA vehicle size classification
- **Format**: String
- **Example**: "Small SUV 4WD"

### Wheelbase_Code
- **Description**: Wheelbase measurement in inches
- **Format**: Decimal number
- **Example**: 115.3

## Status and Pricing

### Miles
- **Description**: Current odometer reading in miles
- **Format**: Integer
- **Value for New Vehicles**: 0
- **Example**: 60081

### SellingPrice
- **Description**: Current asking price for the vehicle
- **Format**: Integer (USD)
- **Example**: 18498

### MSRP. Can be ignored.
- **Description**: Manufacturer's Suggested Retail Price
- **Format**: Integer (USD)
- **Example**: 35000

### BookValue
- **Description**: Estimated book value of the vehicle
- **Format**: Integer (USD)
- **Example**: 18498

### Invoice
- **Description**: Dealer invoice price
- **Format**: Integer (USD)
- **Example**: 32000

### Internet_Price
- **Description**: Special online pricing if available
- **Format**: Integer (USD)
- **Example**: 17995

### Certified
- **Description**: Indicates if vehicle is manufacturer certified pre-owned
- **Format**: Boolean
- **Example**: true/false

## Classification

### MarketClass
- **Description**: Market segment classification of the vehicle
- **Format**: String
- **Example**: "4WD Sport Utility Vehicles"

### PassengerCapacity
- **Description**: Maximum number of passengers
- **Format**: Integer
- **Example**: 5, 7

### Style_Description
- **Description**: Detailed trim level and style information
- **Format**: String
- **Example**: "Signature AWD"

### Options
- **Description**: List of all optional features and equipment
- **Format**: Comma-separated string
- **Example**: "Navigation System, Sunroof, Leather Seats"

---

## Notes
- All monetary values are in CAD
- Null values may be represented as empty strings in CSV format or null in JSON format
- Some fields may be empty or undefined depending on the vehicle's data availability
