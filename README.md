Arlorean/cocos2d
================

TypeScript 0.9 definition for cocos2d/cocos2d-html5, allowing static type checking for web based cocos2d projects.

Example
-------

/// <reference path="cocos2d.d.ts" />

class Helloworld extends cc.Layer {

    helloLabel: cc.LabelTTF = null;
    circle: CircleSprite = null;
    sprite: cc.Sprite = null;

    init(): boolean {
        super.init();
        
        // Your code here
        
        return true;
    }
}


