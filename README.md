Arlorean/cocos2d
================

TypeScript 0.9 definition for cocos2d/cocos2d-html5, allowing static type checking for web based cocos2d projects.

Example
-------

    /// <reference path="cocos2d.d.ts" />

    class CircleSprite extends cc.Sprite {
        _degree = 0;
        constructor() {
            super();
        }
        draw() {
            cc.drawingUtil.setDrawColor4B(255, 255, 255, 255);
    
            if (this._degree < 0)
                this._degree = 360;
            cc.drawingUtil.drawCircle(cc.PointZero(), 30, cc.DEGREES_TO_RADIANS(this._degree), 60, true);
        }
        myUpdate(dt: number) {
            this._degree -= 6;
        }
    }

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


