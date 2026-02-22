# Definition-1
 Write a PL/SQL block which accepts measurement in feet and displays it in cm, inch and meter
 DECLARE
 
    feet   NUMBER:=&feet;
    cm     NUMBER;
    inch   NUMBER;
    meter  NUMBER;
    
BEGIN

    inch  := feet * 12;
    cm    := inch * 2.54;
    meter := feet * 0.3048;
    DBMS_OUTPUT.PUT_LINE('Measurement in Feet  : ' || feet);
    DBMS_OUTPUT.PUT_LINE('Measurement in Inches: ' || inch);
    DBMS_OUTPUT.PUT_LINE('Measurement in CM    : ' || cm);
    DBMS_OUTPUT.PUT_LINE('Measurement in Meter : ' || meter);
    
END;
/
