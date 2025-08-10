# Simple Weather App - Implementation Plan

## Project Overview
Create a simple Python weather application that:
- Uses OpenWeatherMap API to fetch current temperature
- Takes city name as input
- Displays temperature in a clean format
- Follows Basic project structure per data engineering rules

## Implementation Tasks

- [ ] Create Basic project structure (main.py, config.py, test_main.py, planning/todo.md)
- [ ] Set up configuration management with pydantic for API key
- [ ] Create .env.example with OpenWeatherMap API key template
- [ ] Implement weather fetching function with error handling
- [ ] Add main CLI interface for city input
- [ ] Write unit tests for weather functions
- [ ] Create requirements.txt with dependencies
- [ ] Write README.md using our template

## Technical Requirements
- Python 3.11+
- OpenWeatherMap API
- Pydantic for configuration
- Requests for HTTP calls
- Error handling for invalid cities/API failures
- Clean console output

## Success Criteria
- User can enter city name and get current temperature
- Graceful error handling for invalid inputs
- All code follows data engineering best practices
- Tests cover main functionality
- Clear setup instructions in README