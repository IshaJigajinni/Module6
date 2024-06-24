# Module6
# P.1
for line in sys.stdin:
    data = line.strip().split("\t")
    if len(data) == 6:
        date, time, store, item, cost, payment = data
print( "{0}\t{1}".format(item, cost))
# P.2
current_time = datetime.now()
print("Current time:", current_time)
print("Add 1 day:", current_time + timedelta(days=1))
print("Subtract 60 seconds:", current_time - timedelta(seconds=60))
print("Add 2 years:", current_time + timedelta(days=2*365))
# P.3 
delta = timedelta(days=100, hours=10, minutes=13)
print(timedelta:", delta)
# P.4
def inches_height(feet, inches):
    total_inches = feet * 12 + inches
    return total_inches
datetime_object = datetime.now()
print("Current datetime:", datetime_object)
print("type:", type(datetime_object))

feet = 6
inches = 2 
print("Height in inches:", inches_height(feet,inches))
