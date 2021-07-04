# Clear prompt screen:
```python
os.system('cls' if os.name == 'nt' else 'clear')
```

# Run with terminal arguments if called directly: 
```python
if __name__ == "__main__":
    run(sys.argv[1])
```