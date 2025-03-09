if (window.location.pathname === '/en-levels') {
  const tooltipContent = {
  '5': `<div><img src="/images/5.jpg"></div>`,
  '8': `<div><img src="/images/8.jpg"></div>`,
  '11': `<div><img src="/images/11.jpg"></div>`,
  '14': `<div><img src="/images/14.jpg"></div>`,
  '15': `<div><p>Fee Tier Unlock: 0.034% - 0.049%</p></div>`,
  '18': `<div><img src="/images/18.jpg"></div>`,
  '21': `<div><img src="/images/21.jpg"></div>`,
  '24': `<div><img src="/images/24.jpg"></div>`,
  '27': `<div><img src="/images/27.jpg"></div>`,
  '30': `<div><p>Fee Tier Unlock: 0.033% - 0.048%</p></div>`,
  '31': `<div><img src="/images/31.jpg"></div>`,
  '34': `<div><img src="/images/34.jpg"></div>`,
  '37': `<div><img src="/images/37.jpg"></div>`,
  '40': `<div><p>Fee Tier Unlock: 0.032% - 0.047%</p></div>`,
  '41': `<div><img src="/images/41.jpg"></div>`,
  '44': `<div><img src="/images/44.jpg"></div>`,
  '47': `<div><img src="/images/47.jpg"></div>`,
  '50': `<div><p>Fee Tier Unlock: 0.031% - 0.046%</p></div>`,
  '52': `<div><img src="/images/52.jpg"></div>`,
  '55': `<div><img src="/images/55.jpg"></div>`,
  '58': `<div><p>Fee Tier Unlock: 0.030% - 0.045%</p></div>`,
  '61': `<div><img src="/images/61.jpg"></div>`,
  '65': `<div><p>Fee Tier Unlock: 0.029% - 0.044%</p></div>`,
  '72': `<div><p>Fee Tier Unlock: 0.028% - 0.043%</p></div>`,
  '77': `<div><p>Fee Tier Unlock: 0.027% - 0.042%</p></div>`,
  '81': `<div><p>Fee Tier Unlock: 0.026% - 0.041%</p></div>`,
  '84': `<div><p>Fee Tier Unlock: 0.025% - 0.040%</p></div>`,
  '87': `<div><p>Fee Tier Unlock: 0.024% - 0.039%</p></div>`,
  '90': `<div><p>Fee Tier Unlock: 0.023% - 0.038%</p></div>`,
  '93': `<div><p>Fee Tier Unlock: 0.022% - 0.037%</p></div>`,
  '94': `<div><p>PVP T-shirt. Preview coming soon.</p></div>`,
  '96': `<div><p>Fee Tier Unlock: 0.021% - 0.036%</p></div>`,
  '98': `<div><p>Fee Tier Unlock: 0.020% - 0.035%</p></div>`,
  '99': `<div><p>Engraved PVP Ring in 925 sterling silver. Preview coming soon.</p></div>`,
};

  // Function to initialize tooltips on .unlock elements
  function initializeTooltips() {
    const unlockElements = document.querySelectorAll('.unlock:not(.tippy-initialized)');

    if (unlockElements.length > 0) {
      unlockElements.forEach((el) => {
        // Ensure Tippy is only initialized once per element
        tippy(el, {
          content: tooltipContent[el.getAttribute('data-tooltip')] || '<p>No details available.</p>',
          allowHTML: true,
          placement: 'top-start',
          trigger: 'mouseenter',
          animation: 'shift-away-subtle',
          onClickOutside: false,
          hideOnClick: false,
          inertia: true,
          arrow: true,
        });
        el.classList.add('tippy-initialized');
      });
    }
  }

  // Debounce function to limit MutationObserver calls
  function debounce(func, wait) {
    let timeout;
    return function (...args) {
      clearTimeout(timeout);
      timeout = setTimeout(() => func.apply(this, args), wait);
    };
  }

  // Run initially when DOM is fully loaded
  document.addEventListener('DOMContentLoaded', initializeTooltips);

  // Watch for DOM changes with debounced initialization
  const observer = new MutationObserver(debounce(() => {
    initializeTooltips();
  }, 100)); // Adjust delay as needed

  observer.observe(document.body, {
    childList: true,
    subtree: true,
  });

  // Cleanup observer on page unload (optional)
  window.addEventListener('unload', () => observer.disconnect());
}
