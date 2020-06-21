warning! formatting, wordings and grammar mistake ahead
# CFileImage Class
This class serve to read and write png files

## \<constructor>(const string&in path)
Make the CFileImage object "point" to a png image. The string argument represent the path of your image.

All image are created in /Base/Maps/...

the string argument is the path to the png file to which you want to link your CFileImage object to.
It create a CFileImage object that "point" to the file in the specified path. Note that CFileImage uses the CFileMatcher class on the string argument to find the path.
<details>
<summary>Example</summary>
`CFileImage@ myImage = CFileImage("MyModName/"+ map_name + ".png");`
</details>


## \<constructor>(int width, int height, bool has_alpha)
Construct and load a CFileImage object with a specified width, height and specify if the resulting image has alpha (? fact check this).

Usefull when generating image from scratch.
<details>
<summary>Example</summary>
`CFileImage@ myImage = CFileImage(100,75,true);` 

this could be used to create a png file with 100 pixels width and 75 pixel height that has the alpha channel enabled.
</details>


## bool isLoaded()
return a bool value to know weither a image has been loaded into a CFileImage object.
Return true when there's in fact a image loaded into the CFileImage Object
Return false when there's not a image loaded into the CFileImage Object. Usually happen when the CFileImage object cannot find the png file. 
<details>
<summary>Example</summary>

```
CFileImage@ myimage;
if(myimage.isLoaded()){[...]
```

</details>


## void ResetPixel()
clear the currently selected pixel from his value. (probably put the pixel value to 0)
<br>(this is a speculation)<br>


## void canRead()
<br>Check whether or not the loaded file can be read.</br>
<br>return false if it cannot be read</br>
<br>return true if it can be read</br>
<br>(this is a speculation)</br>

## bool nextPixel()
similar to objects with iterator pattern :
Returns true if the CFileImage object has another token in its input and increment the CFileImage offset by 1.
Offset represent which pixel CFileImage is currently "pointing" to. it goes from left to right, top to bottom.
For example, to reach the pixel at (9,1) of a png with the dimension size of 10x10, the index would be 10+9 = 19.
<details>
<summary>Example</summary>
```
usage : CFileImage@ myImage = CFileImage("potatoes.png");
myImage.setPixelOffset(-1);
while(myImage.nextPixel())
{
// do stuff
SColor currentPixel = myImage.readPixel();
}
```
</details>





## SColor readPixel()
Similar to readPixel(uint8&out a, uint8&out r, uint8&out g, uint8&out b) but return the color as a SColor instead of in the given argument. This method doesn't verify if the operation was successful since it doesn't return a bool (assuming the bool value on the other method return the value of canRead())

## bool readPixel(uint8&out a, uint8&out r, uint8&out g, uint8&out b)
Read the current pixel color value using predefined u8 variable. The variable given to the function's arguments are then modified with the corresponding 

<details>
<summary>Example</summary>
```
    if (myImage.isLoaded())
    {
      myImage.setPixelOffset(-1);
      while(myImage.nextPixel())
      {
          u8 a;
          u8 r;
          u8 g;
          u8 b;
          save_image.readPixel(a, r, g, b);
      }
    }
```
</details>



## Vec2f getPixelPosition()
return a Vec2f with the coordinate in  X and Y value of where the CFileImage offset is currently pointing to in the image.
note that (0,0) is in the upper left, not bottom left. incrementing y mean moving downward.


## void setPixelPosition(Vec2f pos)
set the offset of the CFileImage object with coordinate instead of directly with an integer.

(this is a speculation)

## int getPixelOffset()
Get the current offset of the CFileImage Object. The offset is used to determine which pixel the CFileImage object is currently "pointing" to. 

## void setPixelOffset(int pos)
Set the offset of the CFileImage object.

## int getWidth()
return the width of the png that the CFileImage object "point" to.

## int getHeight()
return the Height of the png that the CFileImage object "point" to.

## int getSizeInPixels()

## void setFilename(const string&in filename, ImageFileBase base)
Use this to get your CFileImage object to "point" to your desired png. Filename can be a path, this will create folder in the Maps folder if the path doesn't exist. 

image are created by default in King Arthur's Gold/Base/Maps/yourimage.png.
<details>
<summary>Example</summary>
```
save_image.setFilename("myMod/myImage.png", ImageFileBase::IMAGE_FILENAME_BASE_MAPS);
//do image operation...
save_image.Save();
```
in this example, once Save() is executed on save_image, it will create a png file at 

King Arthur's Gold/Base/Maps/myMod/myImage.png
</details>


## void Save()
Save the current CFileObject image to King Arthur's Gold/Base/Maps/yourimage.png by default or if setFilename has been set, it save it to that location.

## void setPixel(uint8 a, uint8 r, uint8 g, uint8 b)
## void setPixelAndAdvance(uint8 a, uint8 r, uint8 g, uint8 b)
## void setPixel(SColor col)
## void setPixelAndAdvance(SColor col)

## void setPixelAtPosition(uint x, uint y, SColor col, bool blend_alpha)
set pixel at a specific coordinate on the image with the value of the SColor.
blend_alpha serve to activate or deactivate blending between pixels.

## enums
* IMAGE_FILENAME_BASE_MAPS it serve to specify _________
* IMAGE_FILENAME_BASE_CACHE it serve to specify _________

## Variable : 
CFileImage::bool silent_errors

This variable purpose is to _________

## Usage example to load a png file into an array:
```
uint8[][] currentBlueprintData;
int16 currentBlueprintWidth = 0;
int16 currentBlueprintHeight = 0;
void LoadBlueprintFromPng(CRules@ this, string imagePath)
{
	@save_image = CFileImage(imagePath);
	bool done = false;

	if (save_image.isLoaded())
	{
		currentBlueprintWidth = save_image.getWidth();
		currentBlueprintHeight = save_image.getHeight();
		save_image.setPixelOffset(-1);
		uint8[][] _currentBlueprintData(currentBlueprintWidth, uint8[](currentBlueprintHeight, 0));
		currentBlueprintData = _currentBlueprintData;
		u8 a;
		u8 r;
		u8 g;
		u8 b;
		while(save_image.nextPixel() && !done)
		{
			if(save_image.readPixel(a, r, g, b)) ///the argument given are the output of the function
			{
				currentBlueprintData[save_image.getPixelPosition().x][save_image.getPixelPosition().y] = r;
                //in this example, only the red part of the image is used to store something.
                //Therefore only retrieve the red value is retrieved.
			}
			else
			{
				print("an error occured while reading a pixel from a blueprint png");
			}
		}
	}
	else
	{
		print("couldn't load blueprint");
	}
}
```
## Usage example to find all of the images of your mod:
To be able to retrieve all image from your mod, you should prefix or suffix all your image with a identifiers. In this example, every image file wanted has a prefix with "blueprint_".
```
//this is what is executed when saving a file in this example
int currentTime = Time();
save_image.setFilename("DynamicBlueprints/blueprint_" + currentTime + ".png", ImageFileBase::IMAGE_FILENAME_BASE_MAPS);
save_image.setPixelOffset(0);
	//do operations on the image
save_image.Save()
```
The following is a concrete example on how retrieving and loading previously saved image may be implemented : 
```
array<string> filenames;
/* search for all png files path that start with "blueprint_" and
put the path into a string array named filenames */
void searchForBlueprints() 
{
	CFileMatcher@ files = CFileMatcher("blueprint_");
	files.reset();
	while (files.iterating())
	{
		filenames.push_back(files.getCurrent());
		print(files.getCurrent() + " blueprint has been found");
	}
}
```
```
bool loadImage = false; 
void onInit(CRules@ this)
{
	searchForBlueprints(); 
    loadImage = true;
}
```
```
void onTick(CRules@ this)
{

	if(isClient() && loadImage)
	{		
    		/* the following function has been defined in the previous example named
            "Usage example to load a png file into an array:"*/
			LoadBlueprintFromPng(this, filenames[0]); 
            loadImage = false;
	}
}
```
