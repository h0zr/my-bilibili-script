// ==UserScript==
// @name        直播间页面检测到92002自动刷新
// @namespace   Violentmonkey Scripts
// @match       https://live.bilibili.com/*
// @grant       none
// @version     1.0
// @author      -
// @description 2025/2/28 21:03:55
// ==/UserScript==

(function () {
    'use strict';

    document.addEventListener('visibilitychange', () => {
        if (document.visibilityState === 'visible') {
            checkAndReload();
        }
    })

    function checkAndReload() {
        const element = document.querySelector('.web-player-error-code');
        if (element.textContent === 'status: 92002') {
            location.reload();
        }
    }
})();
