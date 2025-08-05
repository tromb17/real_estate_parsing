# 🏠 Real Estate Data Parser

Automated web scraping tool for collecting and analyzing suburban property listings from real estate aggregator.

## 🔍 Project Overview

This Python-based solution extracts detailed property data including:
- Pricing history and metrics (current price, price per sqm, land value)
- Property characteristics (area, year built, floors, amenities)
- Location details (distance from MKAD, highway access)
- Market metrics (views, unique visitors, days on market)

## 🛠️ Technologies Used

- **Web Scraping**: 
  - `Selenium` - For dynamic content loading and interaction
  - `BeautifulSoup` - HTML parsing and data extraction
- **Data Processing**:
  - `Pandas` - Data cleaning, transformation, and analysis
  - `OpenPyXL` - Excel file operations
- **Supporting Libraries**:
  - `re` - Regular expressions for pattern matching
  - `locale` - Localization support
  - `datetime` - Date/time handling

## 🚀 Key Features

1. **Comprehensive Data Collection**:
   - Extracts 40+ data points per property listing
   - Handles both static and dynamic content
   - Captures pricing history and changes

2. **Intelligent Data Processing**:
   - Automated cleaning of raw extracted data
   - Standardization of measurement units (sqm, land area)
   - Special handling for amenities and boolean features

3. **Flexible Output**:
   - Exports structured data to Excel with proper formatting
   - Preserves original listing URLs for reference
   - Ready-to-use dataset for further analysis

## 📊 Data Output Example
| Изменение стоимости ИТОГ | % изменения стоимости | Цена без ЗУ ИТОГ | Цена за 1 кв.м. Без ЗУ ИТОГ | Ссылка | Цена домовладения актуальная | Цена домовладения СТАРТ | Площадь дома | Площадь участка | Кол-во дней в экспозиции | Кол-во просмотров всего | Среднее количество просмотров в 1 день | Среднее в 1 день уникальных | Кол-во уникальных | Состояние дома | Стоимость за 1 кв.м. СТАРТ | Стоимость за 1 кв.м. без ЗУ СТАРТ | Год постройки | Кол-во этажей | Кол-во спален | Кол-во санузлов | Дата выхода в рекламу | Стоимость 1 сотки земли в этом районе | Стоимость ЗУ | Стоимость дома без ЗУ | Газоснабжение | Канализация | Водоснабжение | Категория земель | Статус участка | Материал дома | Шоссе | МКАД | КП |
|--------------------------|-----------------------|------------------|-----------------------------|--------|-------------------------------|-------------------------|--------------|-----------------|---------------------------|--------------------------|----------------------------------------|----------------------------|-------------------|----------------|----------------------------|--------------------------------------|---------------|---------------|---------------|-----------------|-----------------------|--------------------------------------|-------------|----------------------|---------------|-------------|---------------|------------------|----------------|---------------|-------|------|----|
| 8 804 500 RUB | 29% | 29 744 500 RUB | 198 297 RUB/sqm | *** | 38 744 500 RUB | 29 940 000 RUB | 150 m² | 6 | 275 | 172 | 1 | 0 | 84 | - | 199 600 RUB/sqm | 139 600 RUB/sqm | 2025 | 2 | - | 1 | 03.11.2024 | 1 500 000 RUB/сотка | 9 000 000 RUB | 20 940 000 RUB | Есть | Центральная | Есть | - | ИЖС | Газобетонный блок | Калужское, Симферопольское | 32 км | Резиденция Булатово КП |
