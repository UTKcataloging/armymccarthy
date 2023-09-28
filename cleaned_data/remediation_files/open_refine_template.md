# Open Refine Template Army-McCarthy Hearings


## Template

#### Prefix

```
<?xml version="1.0" encoding="UTF-8"?>
<modsCollection xmlns="http://www.loc.gov/mods/v3" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="http://www.loc.gov/mods/v3 http://www.loc.gov/standards/mods/v3/mods-3-5.xsd">
```
####Body

```
<mods>
<identifier type="local">{{cells["FILE NAME"].value}}</identifier>

{{if(isBlank(cells['title'].value), '', '<titleInfo><title>' + cells["title"].value + '</title></titleInfo>')}} 

{{if(isBlank(cells['SPEAKERS 1'].value), '', '<name' + if(isBlank(cells['SPEAKERS 1 URI'].value), '', ' valueURI="' + cells['SPEAKERS 1 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 1'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 2'].value), '', '<name' + if(isBlank(cells['SPEAKERS 2 URI'].value), '', ' valueURI="' + cells['SPEAKERS 2 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 2'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 3'].value), '', '<name' + if(isBlank(cells['SPEAKERS 3 URI'].value), '', ' valueURI="' + cells['SPEAKERS 3 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 3'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 4'].value), '', '<name' + if(isBlank(cells['SPEAKERS 4 URI'].value), '', ' valueURI="' + cells['SPEAKERS 4 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 4'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 5'].value), '', '<name' + if(isBlank(cells['SPEAKERS 5 URI'].value), '', ' valueURI="' + cells['SPEAKERS 5 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 5'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 6'].value), '', '<name' + if(isBlank(cells['SPEAKERS 6 URI'].value), '', ' valueURI="' + cells['SPEAKERS 6 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 6'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 7'].value), '', '<name' + if(isBlank(cells['SPEAKERS 7 URI'].value), '', ' valueURI="' + cells['SPEAKERS 7 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 7'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 8'].value), '', '<name' + if(isBlank(cells['SPEAKERS 8 URI'].value), '', ' valueURI="' + cells['SPEAKERS 8 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 8'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 9'].value), '', '<name' + if(isBlank(cells['SPEAKERS 9 URI'].value), '', ' valueURI="' + cells['SPEAKERS 9 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 9'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 10'].value), '', '<name' + if(isBlank(cells['SPEAKERS 10 URI'].value), '', ' valueURI="' + cells['SPEAKERS 10 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 10'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 11'].value), '', '<name' + if(isBlank(cells['SPEAKERS 11 URI'].value), '', ' valueURI="' + cells['SPEAKERS 11 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 11'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 12'].value), '', '<name' + if(isBlank(cells['SPEAKERS 12 URI'].value), '', ' valueURI="' + cells['SPEAKERS 12 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 12'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['SPEAKERS 13'].value), '', '<name' + if(isBlank(cells['SPEAKERS 13 URI'].value), '', ' valueURI="' + cells['SPEAKERS 13 URI'].value + '"') + '><namePart>' + cells['SPEAKERS 13'].value + '</namePart><role><roleTerm valueURI="http://id.loc.gov/vocabulary/relators/spk">Speaker</roleTerm></role></name>')}}

{{if(isBlank(cells['DATE'].value), '', '<originInfo><dateCreated>' + cells['DATE TEXT'].value + '</dateCreated><dateCreated encoding="edtf">' + cells['DATE'].value + '</dateCreated></originInfo>')}}

{{if(isBlank(cells['Physical Description'].value), '', '<note>' + cells['Physical Description'].value + '</note>')}}

{{if(isBlank(cells['SESSION START TIME'].value), '', '<note>' + cells['SESSION START TIME'].value + '</note>')}}

<physicalDescription><form valueURI="http://vocab.getty.edu/aat/300028633">sound recordings</form><extent>{{cells['DURATION'].value}}</extent>
</physicalDescription>

    <subject valueURI="http://id.loc.gov/authorities/subjects/sh85075833">
        <topic>Legislative hearings</topic>
    </subject>
    <subject valueURI="http://id.loc.gov/authorities/subjects/sh85082515">
        <topic>Army-McCarthy Controversy, 1954</topic>
    </subject>
       <typeOfResource>sound recording-nonmusical</typeOfResource>
    <relatedItem displayLabel="Collection" type="host">
        <titleInfo>
            <title>Recordings of the Army-McCarthy Hearings, 1954</title>
        </titleInfo>
    </relatedItem>
    <relatedItem displayLabel="Collection" type="host">
        <titleInfo>
            <title>Ray H. Jenkins Papers</title>
        </titleInfo>
        <identifier>MPA-0131</identifier>
    </relatedItem>
    <recordInfo>
        <recordContentSource valueURI="http://id.loc.gov/authorities/names/n87808088">University of Tennessee Knoxville. Libraries</recordContentSource>
    </recordInfo>
    <location>
        <physicalLocation valueURI="http://id.loc.gov/authorities/names/no2014027633">University of Tennessee, Knoxville. Special Collections</physicalLocation>
    </location>

    <accessCondition type="use and reproduction" xlink:href="http://rightsstatements.org/vocab/NoC-US/1.0/">No Copyright - United States</accessCondition>
</mods>

```

#### Suffix

```
</modsCollection>
```