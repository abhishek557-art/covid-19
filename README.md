def mock_fetch_covid_data(region):
    # Simulating a response for demonstration purposes
    mock_data = {
        "cases": 100000,
        "recovered": 80000,
        "deaths": 2000
    }
    return mock_data

def get_user_input():
    region = input("Enter a region (country/state/city): ")
    return region

def fetch_covid_data(region):
    # Replace this with the mock function
    return mock_fetch_covid_data(region)

def display_statistics(statistics, region):
    print(f"\nCOVID-19 Statistics for {region.capitalize()}:")
    print(f"Cases: {statistics['cases']}")
    print(f"Recoveries: {statistics['recovered']}")
    print(f"Deaths: {statistics['deaths']}")

def main():
    region = get_user_input()
    statistics = fetch_covid_data(region)

    if statistics:
        display_statistics(statistics, region)
    else:
        print("Error fetching data. Please check the region.")

if __name__ == "__main__":
    main()

Enter a region (country/state/city): india

COVID-19 Statistics for India:
Cases: 100000
Recoveries: 80000
death:2000
